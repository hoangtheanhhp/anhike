# Polkadot là gì
Polkadot được tạo ra bởi Gavin Wood với mục tiêu thiết kế một phiên bản Ethereum phát triển hơn và tương thích với các blockchain biệt lập hiện có như Ethereum và Bitcoin. Vào tháng 8 năm 2019, Polkadot đã ra mắt phiên bản thử nghiệm của nền tảng được gọi là "Kusama". Sau khi khởi chạy Polkadot sẽ hướng tới mục tiêu 100 parachains.

Polkadot tự mô tả mình là một giao thức blockchain thế hệ tiếp theo (thế hệ thứ 3) kết nối một số blockchain chuyên biệt thành một hệ thống / mạng thống nhất.
Các tính năng của Polkadot như sau:
- Promotes interoperability - Thúc đẩy khả năng tương tác: Bằng cách kết nối tất cả các blockchain khác nhau, Polkadot thúc đẩy khả năng tương tác chưa từng có giữa các hệ sinh thái blockchain.
- Scalability - Khả năng mở rộng: Một tập hợp validator tiêu chuẩn có thể vận hành nhiều blockchain được kết nối qua Polkadot. Điều này giúp tăng khả năng mở rộng theo cấp số nhân
- Innovation - Đổi mới sáng tạo: Khung nền của Polkadot cho phép bạn tạo blockchain tùy chỉnh một cách dễ dàng. Nhờ đó, nhiều nhà phát triển tham gia vào hệ thống hơn.
- Removing forks - Loại bỏ fork: Forks có thể gây ra sự tàn phá và chia rẽ cộng đồng (chỉ cần hỏi Bitcoin và Ethereum). Polkadot có thể tích hợp các tính năng mới, sửa lỗi và nâng cấp mà không cần fork.
- Better security - Bảo mật tốt hơn: Polkadot cho phép các chuỗi tương tác với nhau trong khi vẫn đủ khả năng vận hành, quản lý độc lập.

# Cấu trúc Polkadot
- Một số khái niệm:
  - Relaychain: Là chuỗi căn bản của Polkadot có khả năng kết nối các chuỗi riêng lẻ và giải quyết các vấn đề tương tác giữa các chuỗi đó.
  - Parachain: Viết tắt của parallelized chains(chuỗi song song) giải quyết vấn đề mở rộng mạng lưới nhờ việc chạy song song.
  - Bridge Chain: Kết nối với các Blockchain khác ko sử dụng Polkadot Protocol

![Polkadot](https://academy.ivanontech.com/wp-content/uploads/2021/06/relaychain.png)

# Giao thức Polkadot
![Polkadot](https://academy.ivanontech.com/wp-content/uploads/2021/06/protocols-1024x403.png)

Polkadot hiện đang chạy một một phiên bản của Proof of Stake là “nominated proof of stake” được giải thích như dưới đây
- Validator bảo mật relay chain bằng việc staking DOT tokens
- Validator cũng tham gia vào quá trình đồng thuận bằng cách tham gia đồng thuận với những validator khác và xác thực bằng chứng của collator - người đối chiếu.
- 