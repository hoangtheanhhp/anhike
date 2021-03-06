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

Sổ lệnh tự động trên chuỗi - Automated on-chain limit orderbooks cho phép người dùng thực hiện các lệnh giao dịch một các trực tiếp bao gồm chọn được mức giá và khối lượng giao dịch. Và điều tuyệt vời là nó là phi tập trung, tất cả giao dịch đều được minh bạch.
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

7. WinDEX Fiat
   WinDEX Fiat sẽ làm cho WinDEX Orderbook trở thành sàn giao dịch tiền điện tử phi tập thu hút được người dùng từ thị trường tài chính truyền thống. Các sàn DEX hiện tại chỉ tập trung phát triển nền tảng giao dịch cho những người sở hữu tiền điện tử vì không cung cấp KYC. Chúng tôi sẽ trở thành dự án kết nối thị trường tài chính truyền thống với thế giới tiền điện tử phi tập trung.
   winDEX cho phép các nhà giao dịch:
	- Mua crypto thông qua thẻ tín dụng hoặc tài khoản ngân hàng.
	- Nhận token trực tiếp trong ví của người dùng mà không bị giám sát.

9. Decentralized KYC - Xác thực danh tích phi tập trung
	- Trên các nền tảng phi tập trung, các nhà giao dịch có thể giao dịch với nhau mà không cần xác định danh tính. Tuy nhiên trong thời điểm hiện tại, việc này hạn chế số lượng người dùng tham gia vào các sàn giao dịch phi tập trung. Chính vì thế chúng tôi đưa ra giải pháp Decentralized KYC - Xác thực danh tích phi tập trung. Bằng cách dụng bằng chứng mật mã thay vì thông tin chính danh của người dùng để xác minh. Chúng tôi có thể ngăn chặn được các hành vi rửa tiền hoặc các hình thức phạm tội tài chính khác.
10. WinDEX NFTs
    - Đây là tính năng bổ sung cho hệ sinh thái của WinDEX cacs NFT sinh ra có cơ chế làm phần thưởng cho người tham giao dịch tích cực trên mạng lưới.
11.	WinDEX P2P Lending
	- P2P Lending (Cho vay ngang hàng) là hình thức cho vay trực tiếp giữa người vay và người cho vay mà không cần thông qua một bên thứ 3 làm trung gian.
	- Cụ thể, bằng cách sử dụng các Smart Contract, người đi vay và người cho vay có thể ký hợp đồng cho vay và đi vay mà không cần thông qua trung gian. Thay vào đó, các Smart Contract tự thực hiện và cho phép giao dịch.
	- Ưu điểm lớn nhất của P2P Lending là chi phí và lãi suất cho vay thấp hơn rất nhiều so với 2 hình thức còn lại vì loại bỏ được bên trung gian. Nhờ đó mà thông tin giao dịch và khách hàng cũng được đảm bảo tính bảo mật.

12.	WinDEX feature
	- Giao dịch feature là không thể thiếu đối với các sàn giao dịch tập trung, chúng tôi sẽ dưa mô hình này lên sàn giao dịch phi tập trung WinDEX để tăng cơ hội kiếm lợi nhuận cho các nhà giao dịch trong thị trường tiền mã hóa.

1.  WinDEX team
	- Hoàng Thế Anh là một kỹ sư tốt nghiệp từ trường Đại học Bách Khoa Hà Nội, có đam mê công nghệ, đặc biệt trong lĩnh vực blockchain. Tham gia nghiên cứu trong các group blockchain hàng đầu Việt Nam như Vietnam Blockchain Innovation và Diamond NetWork. Dựa trên nhũng kiến thức nền tảng về Systems engineering, tôi quyết tâm xây dựng mạng lưới Blockchain đầy đủ tính năng và đảm bảo sự bảo mật tuyệt đối. Kiến thức trang bị  Python, RUST & Substrate Framework.


Mô hình kinh doanh
- Giá trị nội tại của WinDEX là xây dựng hệ sinh thái sàn giao phi tập trung trên một blockchain riêng biệt. Chính vì thế đồng coin WID tăng cùng với sự phát triển của WinDEX theo chiều dài thời gian. Điều chúng tôi hướng đến là một thị trường giao dịch phi tập trung, nơi đó mọi lợi nhuận thu được từ chi phí giao dịch của người dùng đều đóng góp vào kho bạc của dự án, không có bất cứ cá nhân nào sở hữu số lợi nhuận thu được từ đó. Chính điều này làm tăng giá trị nội tại của WinDEX.
- Các mô hình thu lợi nhuận
  - 50% phí giao dịch người dùng sẽ đóng góp vào kho bạc.
  - Thu lợi nhuận từ hoa hồng cho việc ghép nối người vay và người cho vay trong P2P Leading
  - Lợi nhuận từ giao dịch phái sinh sẽ đóng góp 100% vào dự án
  - Có hai loại lệnh trên WinDEX - Lệnh Maker là lệnh không thực hiện ngay lập tức và nằm yên trên sổ lệnh - những lệnh này bổ sung độ sâu và tính thanh khoản cho sổ lệnh. Mặt khác, lệnh Taker lấp đầy ngay các lệnh Maker hiện có. Họ xóa thanh khoản từ sổ lệnh.
Để giảm thiểu chi phí giao dịch, chúng tôi sẽ tính phí cao hơn cho các đơn đặt hàng nhỏ hơn các đơn đặt hàng lớn hơn. Phía Maker sẽ không tính phí 0 để khuyến khích người dùng mở các lệnh giới hạn trên sổ đặt hàng.
- Money trading volume https://miro.medium.com/max/875/0*gKuayb87Ak0sMtHV
- https://miro.medium.com/max/3000/1*XL7pFU_q0QHyiqY_ZN9sDQ.png




Nhằm giảm bớt độ phức tạp, tăng tốc độ giao dịch cũng như loại bỏ những dữ liệu không cần thiết trên chuỗi chính, WinDEX tin rằng chỉ những dữ liệu công khai mới cần thiết lưu trữ trên chuỗi

Windex đưa ra cơ chế off-chain state commit

Những dữ liệu cần xác thực công khai như tài sản người dùng mới được đẩy lên chain

Những dữ liệu khác như sổ lệnh giao dịch, chỉ số dữ liệu thị trường, dữ liệu lịch sử giao dịch... sẽ được lưu trữ off-chain

Dữ liệu off-chain sẽ được xây dựng như một lớp layer 2, để đảm bảo tính bảo mật và minh bạch cho hệ thống

Điều này giúp cho hệ thống tăng khối lượng, giảm độ trễ giao dịch cũng như cạnh tranh trực tiếp với sàn tập trung

3: Mô hình kinh doanh : 1’ -> Thế Anh
Giá trị của WinDEX được tích lũy theo thời gian hoạt động. Chủ yếu là từ phí giao dịch.
WinDEX cung cấp 2 loại lệnh là limit order và market order. Với lệnh market order phí giao dịch sẽ là 0.2%, lệnh limit order phí giao dịch bằng 0. Nhằm khuyến khích các nhà tạo lập thì trường trên hệ thống. Phí giao dịch thu được sẽ được chia 50:50. 50% được trả cho nhà tạo lập thì trường và 50% đưa vào kho bạc của WinDEX. Do đó chi phí giao dịch được tích tụ vào đồng coin WID, nên giá trị của nó ngày càng tăng theo khối lượng giao dịch và tăng theo quy mô của thị trường.Và lợi nhuận của WinDEX không bị nắm giữ bởi chủ sàn mà nằm trong tay người dùng thông qua việc nắm giữ đồng coin WID
Ngoài ra Giá trị WinDEX có được từ một số tính năng:
-Thu được phí giao dịch từ việc cho vay và môi giới cho vay. Người cho vay thu được lợi nhuận thông qua việc cho vay thông qua WinDEX.
-Hỗ trợ launchpad, cho các dự án cần huy động vốn. WinDEX coin sẽ bị khoá để có thể tham gia các dự án này, tạo ra sự khan hiếm làm tăng giá trị của WinDEX
...vv
4: Các chức năng sẽ được xây dựng: 20s
-	Nhằm đáp ứng nhu cầu về dòng tiền trong tương lai, dự án sẽ phát triển các tính năng như sau: Chức năng tạo thanh khoản, chức năng vay và cho vay, chức năng giao dịch sử dụng đòn bẩy.
-	Với mục tiêu giảm chi phí và mở rộng, dự án sẽ hướng tới là 1 parachain của Polkadot, khi đó các cầu nối tới các hệ sinh thái khác sẽ trở nên rẻ và hấp dẫn hơn
-	Oracle cũng được sử dụng nhằm mục đích cập nhật thông tin giá cả một cách an toàn, giúp tránh được những vụ tấn công chênh lệch giá

