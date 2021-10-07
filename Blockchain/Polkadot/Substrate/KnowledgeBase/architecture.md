
# Architecture

![architecture](https://substrate.dev/docs/assets/substrate-arch.png)

The Substrate client is an application that runs a Substrate-based blockchain node. It consists of several components that include, but are not limited to, the following:

Substrate Client là một ứng dụng chạy một node blockchain dựa trên Substrate. Nó bao gồm một số thành phần bao gồm (nhưng không giới hạn) những thành phần sau:

- Storage: được sử dụng để duy trì trạng thái phát triển của một Subtrate Blockchain. Mạng lưới blockchain cho phép người tham gia đạt được sự đồng thuận không tin cậy về trạng thái lưu trữ. Substrate vận chuyển với cơ chế lưu trữ key-value đơn giản và hiệu quả cao.
- 
Runtime: logic định nghĩa các block được xử lý thế nào, bao gồm cả logic chuyển đổi. Trong Substrate, mã runtime đc biên dithe logic that defines how blocks are processed, including state transition logic. In Substrate, runtime code được biên dịch thành Wasm và trở một phần trạng thái lưu trữ của blockchain. Điều này cho phép một trình năm của blockchain dựa trên Substrate: nâng cấp mà ko cần fork-forkless runtime upgrades. Substrate clients cũng có thể chứa "native runtime" - được biên dịch giống với nền tảng client. The component of the client that dispatches calls to the runtime is known as the executor, whose role is to select between the native code and interpreted Wasm. Although the native runtime may offer a performance advantage, the executor will select to interpret the Wasm runtime if it implements a newer version.
Peer-to-peer network: the capabilities that allow the client to communicate with other network participants. Substrate uses the Rust implementation of the libp2p network stack to achieve this.
Consensus: the logic that allows network participants to agree on the state of the blockchain. Substrate makes it possible to supply custom consensus engines and also ships with several consensus mechanisms that have been built on top of Web3 Foundation research.
RPC (remote procedure call): the capabilities that allow blockchain users to interact with the network. Substrate provides HTTP and WebSocket RPC servers.
Telemetry: client metrics that are exposed by the embedded Prometheus server.