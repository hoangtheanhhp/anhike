Serum

Introduction
	What is this?
CEX
DEX
OrderBook
Bridge
Substrate
Tổng quan về WinDex
Liệt kê các chức năng Project sẽ thực hiện
- Sàn DEX tích hợp OrderBook(tham khảo serum)
- Token/coin phát hành tên già gì?
- Chức năng Swap có tính năng gì nổi bật? có kết nối với ecosystem khác không, nếu có thì như thế nào?
- ...


 Tác dụng của đồng coin/token và tokenomic
	-> Tham khảo phần người hold coin/token sẽ có lợi thế gì?
	Phần tokenomic nên tách riêng làm 1 mục


1. OrderBook của WinDex (Mục này tham khảo mục 5 của Serum)

2. Roadmap v2 (không có trong whitepaper)
Chia làm 3 phase
Phase One
2020 launched
Ra mắt sàn giao dịch DEX on-chain
Cung cấp thanh khoản
Phase Two
Cross-chain
Ra mắt wallet
Serum Swap
Phase Three
Serum Swap được build trực tiệp trên OrderBook không phải AMM
Staking
Thêm TradingView Chart

-> Mục roadmap anh em tự nghĩ rồi viết cũng được.
Roadmap của serum nhìn không được hay cho lắm

Điểm còn thiếu của Whitepaper này
Chưa nêu rõ business model
Chưa nếu các công nghệ nổi bật sử dụng trong project
Chưa nói rõ cơ chế swap cross-chain


1.4 Orderbooks
Uniswap đã lặng lẽ cách mạng hóa thế giới DeFi bằng cách cho phép giao dịch mà không cần sổ lệnh - Orderbooks.

Nhưng điều đáng chú ý hơn cả là việc tạo ra thị trường tự động Automated Market Makin (AMM) rất cần thiết. AMM là một hệ thống không có các lệnh giao dịch giới hạn hay lệnh chào bán, lệnh chào mua. Trong một sổ lệnh, bạn có thể quyết định được mức giá, khối lượng giao dịch một cách chủ động. Do đó, có rất nhiều điểm hạn chế của các sàn giao dịch AMM. Bạn không thể cung cấp thanh khoản trừ phi bạn cung cấp cho cả 2 bê(bán-mua). Bạn không thể chọn mua chỉ ở một mức giá cụ thể, bạn không thể cung cấp mức giá bán nào khác ngoài mức giá của thị thường, và bạn không thể quyết định được khối lượng giao dịch.

Sổ lệnh giao dịch giải pháp giải quyết vấn đề này. Nhưng hiện nay DeFi không có sổ lệnh giao dịch bởi gì nó khó có thể hoạt động trên mạng lưới ETH quá chậm và đắt đỏ.

5. Order Book

Sổ lệnh tự động trên chuỗi - Automated on-chain limit orderbooks cho phép người dùng thực hiện các lệnh giao dịch một các trực tiếp bao gồm chọn được mức giá và khối lượng giao dịch. Và điều tuyệt vời là nó là phi tập chung, tất cả giao dịch đều được minh bạch.
Sổ lệnh trên DeFi hoạt động on-chain do đó phải có sự tính toán sao cho nó nhanh hơn và rẻ hơn.

WinDEX Orderbook là sản phẩm chủ đạo của chúng tôi. Đó là một sản phẩm giao dịch phi tâp trung Layer 2 được xây dựng trên mạng lưới Polkadot Network tích hợp tính năng của một orderbook. Có 2 nhóm nhà giao dịch chính:
	- Những nhà giao dịch truyền thống họ chấp nhận rủi ro, gửi tài sản của mình lên các sàn tập trung để thực hiện giao dịch một các nhanh chóng và các thao tác thân thiện với người dùng.
	- Những nhà giao dịch trên nền tảng phi tập trung bỏ qua được những rủi ro liên quan đến quản lí tài sản, họ phải đánh đổi bằng một số vấn đề liên quan đến giao dịch và sự hạn chế của chức năng giao dịch phi tập trung.

Windex giữa lại tất cả sự tiện lợi của giao dịch tập trung và phi tập trung.

WinDex orderbook mang đến cho người dùng các tính năng giao dịch không giới hạn như sau:
	- Mức độ bảo mật cả nhất cho các khoản đầu tư của người dùng.
	- Tốc độ giao dịch lên tới 500000 giao dịch/ giây với độ trễ khoảng 20 mili giây.
	- Không phí gas
	- Khả năng tương tác qua lại giữa các blockchain
	- Hỗ trợ thanh khoản cross-chain
	- Loại bỏ front-running trong giao dịch
	- Tăng cường các chức năng giao dịch bao gồm giao dịch tầng suất cao
	- Tích hợp API tốc độ cao nhằm phục vụ các nhà tạo lập thị trường và bot giao dịch
	- Mang đến sự tiện lợi thông qua đa nền tảng bao gồm cả web và mobile app
	- Cơ hội mua crypto trực tiếp từ tiền fiat
Nếu là một nhà giao dịch trên WinDEX chắc chắn rằng bạn sẽ cảm thấy tuyệt vời vì những tính năng chúng tôi mang lại.


5. Windex Orderbook Architecture
   Chúng tôi tích hợp nhiều công nghệ cho WinDEX để tăng cường bảo mật cho mạng lưới như: WinDEX Network blockchain, Trusted Execution Environments(TEE), Orderbook Engine, IPFS.
	- WinDEX Network là một mạng lưới blockchain độc lập được xây dựng trên Substrate kế thừa nền tảng bảo mật của Polkadot
	- Trusted Execution Environment (TEE)
	- Orderbook Engine duy trì một số lệnh hiệu suất cao, ghép nối các giao dịch và cung cấp TEE cho việc xác thực.
	- IPFS
	- Diagram - https://docs.polkadex.trade/assets/images/orderbookBanner-b6e5342dbae5eafcae07eac56043acc3.jpg

6. Lợi ích
   Windex cung cấp cho những người dùng muốn có trải nghiệm giao dịch tốt nhất nhưng vẫn có sự đảm bảo cao nhất về bảo mật.
	- Cho phép các nhà giao dịch tích hợp nhiều ví cá nhân on-chain
	- Sử dụng Windex orderbook các nhà giao dịch có thể ủy thác tài sản giao dịch cho bên thứ ba ( như bot trading) để có thể thu lợi từ các thuật toán giao dịch
	- Windex Orderbook cho phép thực hiện các giao dịch mua bán với số lượng lớn.
	- Các nhà giao dịch hoàn toàn có thể an tâm để tài sản trên sàn mà không lo các sàn bị hack. Bởi vậy giảm được phí giao dịch khi chuyển tài sản qua lại.
	- Các nhà giao dịch có thể mua bán trực tiếp bất kì token ERC-20 hoặc token trên các dự án Substrate khác khi WinDEX trở thành một parachain.

6. Polkadex IDO PlatForm
Ngày công nghiệp tiền mã hóa đang ngày càng phát triển cả về số lượng dự án lẫn số lương người dùng.
Các nhà đầu tư muốn tham gia vào các dự án tiềm năng một cách sớm nhất từ đó thu được lợi nhuận khủng lồ dựa trên tỉ lể tăng trưởng của các dự án.
Tham gia IDO cần rất nhiều thời gian và sự kiên nhẫn
Các vấn đề hiện tại của các nền tảng phân phối token là:
	- Các nền tảng IDO vẫn mang nặng tính tập trung, dựa trên hình thức xổ số để phân phối token.
	- Whitelisting và smart contract để phân phối token trên mạng lưới ETH cực kì đắt đỏ vì phí gas cao.
	- Các nhà đầu tư muốn tham gia IDO phải nắm giữ số lượng lớn token nền tảng, điều này hạn chế các nhà đầu tư nhỏ lẻ tham gia vào IDO.
WinDEX platform sẽ cũng cấp các tính năng phân phối to

10. WinDEX team
	- Hoàng Thế Anh là một kỹ sư tốt nghiệp từ trường Đại học Bách Khoa Hà Nội, có đam mê công nghệ, đặc biệt trong lĩnh vực blockchain. Tham gia nghiên cứu trong các group blockchain hàng đầu Việt Nam như Vietnam Blockchain Innovation và Diamond NetWork. Dựa trên nhũng kiến thức nền tảng về Systems engineering, tôi quyết tâm xây dựng mạng lưới Blockchain đầy đủ tính năng và đảm bảo sự bảo mật tuyệt đối. Kiến thức trang bị  Python, RUST & Substrate Framework.

