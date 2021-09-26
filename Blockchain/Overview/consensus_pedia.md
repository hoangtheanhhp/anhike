# Cơ chế đồng thuận trong Blockchain
Cơ chế đồng thuận là một cơ chế giúp các nhà giao dịch đưa ra các thỏa thuận mà không gặp vấn đề gì về lợi ích, mong muốn ảnh hưởng của các nhóm thiểu số. Đồng thời, đảm bảo rằng 1 nhóm nào đó không thể dùng quyền của mình để áp đặt hay điều khiển cả một tổ hợp người dùng trên cùng mạng lưới.

![Cơ chế đồng thuận của Blockchain](https://lina.network/wp-content/uploads/2020/07/consensus-mechanisms.jpg)

*Cơ chế đồng thuận của Blockchain*

Cơ chế đồng thuận chịu trách nhiệm duy trì tính toàn vẹn và bảo mật của hệ thống phân tán. Khi một giao dịch được diễn ra, hệ thống trên Blockchain sẽ gửi thông tin đến các nút cá nhân. Giao dịch chỉ được diễn ra khi nhận được nhiều sự đồng thuận hơn từ các nút cùng trong mạng lưới đó.

Hiện nay, nền tảng blockchain có hai cơ chế đồng thuận chính: đồng thuận bằng Bằng chứng công việc (Proof of Work) và Bằng chứng cổ phần (Proof of Stake). Ngoài ra còn rất nhiều các thuật toán đồng thuận khác sẽ được giới thiệu ở dưới đây

1. Proof of Work

![image](https://miro.medium.com/max/1204/1*AqgfTthyFsFAxHhXxa7NEg.png)

- Ưu điểm:
Nó đã được thử nghiệm từ năm 2009 và vẫn đứng vững cho đến ngày nay.
- Nhược điểm:
    - Tốc độ xử lý chậm.
    - Sử dụng nhiều năng lượng, không tốt cho môi trường.
    - Dễ bị ảnh hưởng bởi quy mô nền kinh tế.
    - Được sử dụng bởi: Bitcoin, Ethereum, Litecoin, Dogecoin, v.v.
- Loại hình: Đồng thuận cạnh tranh.
- Giải thích: 
>Đây là thuật toán đồng thuận đầu tiên (được đề xuất bởi Satoshi Nakamoto cha đẻ của Bitcoin) để tạo ra sự đồng thuận phân tán và giải quyết vấn đề chi tiêu gấp đôi. POW không phải là một ý tưởng mới, nhưng cách Satoshi kết hợp điều này và các khái niệm hiện có khác - chữ ký số, chuỗi merkle và mạng P2P - thành một hệ thống đồng thuận phân tán khả thi, trong đó tiền điện tử là ứng dụng cơ bản và đầu tiên, khá sáng tạo.
Cách thức hoạt động mà những người tham gia blockchain (được gọi là thợ đào) phải giải quyết một vấn đề tính toán phức tạp nhưng vô dụng để thêm một khối giao dịch vào blockchain.

2. Proof of Stake
- Ưu điểm:
    - Tiết kiệm năng lượng.
    - Muốn tấn công mạng phải bỏ ra chi phí lớn để thu gom coin/token.
    - Không dễ bị ảnh hưởng bởi quy mô kinh tế
- Nhược điểm:
    - Vấn đề [nothing at stake](https://kipalog.com/posts/Tim-hieu-Proof-of-Stake--Nothing-at-Stake) (cổ phần bằng 0)

- Được sử dụng bởi: Ethereum (v2), Peercoin, Nxt.
- Loại hình: Đồng thuận cạnh tranh.
- Giải thích: 
>Bằng chứng cổ phần được tạo ra để thay thế cho bằng chứng công việc (PoW), để giải quyết các nhược điểm của PoW. Ở đây thay vì sử dụng khai thác, bạn phải có một số cổ phần (coins) trong hệ thống. Vì vậy, nếu bạn sở hữu 10% cổ phần (tiền xu), thì xác suất khai thác khối tiếp theo của bạn sẽ là 10%.
Mining đòi hỏi rất nhiều sức mạnh tính toán để chạy các tính toán mật mã khác nhau nhằm giải quyết các thách thức tính toán. Sức mạnh tính toán chuyển thành một lượng điện cao và năng lượng cần thiết cho việc chứng minh công việc. Vào năm 2015, người ta ước tính rằng một giao dịch Bitcoin yêu cầu lượng điện cần thiết để cung cấp năng lượng cho 1,57 hộ gia đình Mỹ mỗi ngày. Vì vậy, để tiết kiệm điện năng, PoS đã được giới thiệu.

>Trong PoS, một đô la là một đô la. Ví dụ(so sánh với PoW): hãy xem xét 10.000 miners, mỗi người chi tiêu 1$/phút (87,6M$/năm) có thể có ít sức mạnh băm hơn một nhóm miners chi 10.000$/phút (mặc dù cũng chi tiêu 87,6M$/năm). Nhưng trong trường hợp PoS, bạn không thể sử dụng hết nó cùng một lúc. Ở đây một đô la là một đô la. Do đó, nó không dễ bị ảnh hưởng bởi lợi thế quy mô.

>Ngoài ra, tấn công một hệ thống PoS đắt hơn tấn công một hệ thống PoW. 
Điều này có nghĩa là bạn mất số cổ phần(coins) khi bạn thực hiện một cuộc tấn công vào hệ thống PoS, trong khi trong PoW, bạn không mất thiết bị khai thác hoặc tiền của mình nếu bạn tấn công hệ thống; thay vào đó, bạn chỉ làm cho nó (tấn công một hệ thống PoW) khó thực hiện.
Nhưng một vấn đề có thể phát sinh là vấn đề “nothing-at-stake”, trong đó các trình tạo khối không có gì để mất bằng cách bỏ phiếu cho nhiều lịch sử blockchain (các nhánh forks), do đó ngăn cản sự đồng thuận đạt được.

![nothing-at-stake](https://hackernoon.com/hn-images/0*rBz8CQGfVrCxTivc.png)
*Trong PoS, bạn có thể stake tài sản của mình ở cả hai bên của chuỗi (vấn đề “nothing-at-stake”) trong khi trong PoW, bạn không thể khai thác cả hai bên (vì nó quá khó)*

Bởi vì không giống như trong các hệ thống bằng chứng công việc (nơi bạn phải tính toán rất nhiều để mở rộng một chuỗi), có rất ít chi phí để làm việc trên một số chuỗi. Nhiều dự án đã cố gắng giải quyết vấn đề này theo những cách khác nhau. Ví dụ. như đã nêu ở trên, một trong những giải pháp là trừng phạt những validators xấu.



3. Delayed Proof-of-Work

- Ưu điểm:
    - Tiết kiệm năng lượng
    - Tăng cường bảo mật
    - có thể gia tăng giá trị cho các blockchain khác bằng cách gián tiếp cung cấp bảo mật cho Bitcoin mà không phải trả chi phí giao dịch Bitcoin
- Nhược điểm:
    - Chỉ các blockchain sử dụng PoW hoặc PoS mới có thể là một phần của sự đồng thuận này.
    - Trong chế độ “Hoạt động công chứng”, tốc độ băm cho các node khác nhau (node công chứng và node bình thường) phải được hiệu chỉnh, nếu không, sự khác biệt giữa các tốc độ băm có thể bùng nổ (xem bên dưới để giải thích thêm)
- Được sử dụng bởi: Komodo
- Loại: Đồng thuận hợp tác
- Giải thích: 
>Bằng chứng công việc bị trì hoãn (dPoW) là một phương pháp đồng thuận kết hợp cho phép một blockchain tận dụng lợi thế của bảo mật được cung cấp thông qua sức mạnh băm của một blockchain thứ cấp. Điều này đạt được thông qua một nhóm các node công chứng bổ sung dữ liệu từ blockchain đầu tiên vào blockchain thứ hai, sau đó sẽ yêu cầu cả hai blockchains bị xâm phạm để làm suy yếu tính bảo mật của blockchain đầu tiên. Tiên sử dụng phương pháp đồng thuận này là Komodo, được gắn với chuỗi khối Bitcoin.

![dPoW](https://hackernoon.com/hn-images/0*mAL25OaVAr-1Jzvf)
*dPoW*

>Blockchain dựa trên dPoW có thể sử dụng các phương pháp đồng thuận Proof of Work (PoW) hoặc Proof of Stake (PoS) để hoạt động; và nó có thể tự gắn vào bất kỳ blockchain PoW nào mong muốn. Tuy nhiên, tỷ lệ băm của Bitcoin hiện cung cấp mức độ bảo mật cao nhất cho các blockchain được bảo mật bằng dPoW. Hình minh họa bên dưới cho thấy mối quan hệ của các bản ghi riêng lẻ với chuỗi khối chính và chuỗi khối PoW đính kèm của nó:

![dPoW](https://hackernoon.com/hn-images/1*rfxNiaL3KpCPFgvFCsvpHw.png)

*dPoW*

>Có hai loại node trong hệ thống dPoW: node công chứng(notary node) và node bình thường (normal node). 64 node công chứng được các bên liên quan trong chuỗi khối dPoW bầu chọn để thêm (công chứng) các khối đã được xác nhận từ chuỗi khối dPoW vào chuỗi khối PoW đính kèm. Khi một khối đã được hoàn thành, chuỗi băm của nó được thêm vào giao dịch Bitcoin được ký bởi 33 trong số các node công chứng, tạo ra bản ghi về các băm khối dPoW trên chuỗi khối Bitcoin đã được công chứng bởi phần lớn các node công chứng của mạng.
Để ngăn chặn cuộc chiến khai thác giữa các node công chứng, điều này sẽ làm giảm hiệu quả của mạng, Komodo đã nghĩ ra một phương pháp khai thác vòng tròn hoạt động trên hai chế độ. Chế độ “No Notary - Không có công chứng” cho phép tất cả các node mạng khai thác các khối, tương tự như cơ chế đồng thuận PoW truyền thống. Tuy nhiên, trong chế độ “Hoạt động của Công chứng viên”, các công chứng viên mạng sẽ khai thác với tỷ lệ độ khó mạng giảm đáng kể. Trong chương trình này, mỗi công chứng viên được phép khai thác một khối với độ khó hiện tại của nó, trong khi các node công chứng khác phải khai thác ở mức cao hơn 10 lần và tất cả các node bình thường sẽ luôn khai thác ở mức độ khó gấp 100 lần tỷ lệ khó của các node công chứng.
Nhưng điều này gây ra một số vấn đề. Như đã đề cập trong một cuộc trò chuyện của tôi với người sáng lập Komodo, nó có thể dẫn đến sự khác biệt cao giữa hashrate của những người khai thác công chứng(notary miners) và những người khai thác bình thường(normal miners)

>Hệ thống dPoW được thiết kế để cho phép blockchain tiếp tục hoạt động mà không cần các node công chứng. Trong tình huống như vậy, blockchain dPoW có thể tiếp tục hoạt động dựa trên phương pháp đồng thuận ban đầu của nó; tuy nhiên, nó sẽ không còn có tính bảo mật bổ sung của chuỗi khối đính kèm.

![dPoW](https://hackernoon.com/hn-images/1*6Qq08zfbxgg6fYz6l3yq8w.png)

>Do đó, Bằng chứng công việc trì hoãn cho phép tăng cường bảo mật và giảm mức sử dụng năng lượng cho bất kỳ chuỗi khối nào sử dụng phương pháp đồng thuận này. Ví dụ: vì Komodo sử dụng thuật toán băm Equihash để ngăn chặn việc khai thác bằng [ASIC](https://vi.gadget-info.com/84547-what-is-asic-and-how-it-has-taken-over-bitcoin-mining) và nó dựa trên phương pháp khai thác vòng tròn cho các node công chứng, các biện pháp khuyến khích được cấu trúc để giảm khả năng cạnh tranh giữa các node sẽ dẫn đến việc sử dụng quá nhiều năng lượng hoặc tính toán sức mạnh.

>Ngoài ra, một chuỗi khối dPoW như Komodo có thể tăng giá trị cho các chuỗi khối khác bằng cách gián tiếp cung cấp bảo mật Bitcoin mà không phải trả chi phí giao dịch Bitcoin: Một chuỗi khối thứ ba sử dụng dPoW có thể tự gắn với Komodo, sau đó được gắn với Bitcoin. Bằng cách này, các chuỗi khối dPoW có thể được hưởng lợi từ tỷ lệ băm cao của Bitcoin mà không cần phải gắn trực tiếp vào chuỗi khối Bitcoin.

>Cuối cùng, các chức năng được tách biệt của các node công chứng và các node bình thường trong hệ thống đảm bảo rằng cơ chế đồng thuận ban đầu tiếp tục hoạt động trong trường hợp các node công chứng bị lỗi. Sự phụ thuộc lẫn nhau này tạo ra động lực cho các mạng khác hỗ trợ việc duy trì liên tục mạng Bitcoin mà không hoàn toàn phụ thuộc vào chức năng trực tiếp của nó.

4. Delegated Proof-of-Stake
![dPoS](https://ucarecdn.com/2c41d5d7-20f6-47bf-8e99-160b7a0c14f1/)

- Ưu điểm:
    - Tiết kiệm năng lượng.
    - Nhanh. 
- Nhược điểm:
    - Có một chút tập trung.
    - Những người tham gia có lượng staking cao có thể tự bỏ phiếu để trở thành validator. 
- Được sử dụng bởi: BitShares, Steemit, EOS, Lisk, Ark
- Loại: Đồng thuận hợp tác
- Giải thích: 
>Trong DPoS, những người có liên quan trong hệ thống có thể bầu ra các nhà lãnh đạo (nhân chứng), những người sẽ bỏ phiếu thay cho họ. Điều này làm cho nó nhanh hơn PoS bình thường.

>Ví dụ. trong trường hợp EOS, 21 nhân chứng được bầu chọn cùng một lúc và một nhóm các node (nhân chứng tiềm năng) được giữ ở chế độ chờ để nếu ai đó trong các node nhân chứng chết hoặc thực hiện một số hoạt động độc hại, thì nó có thể được thay thế bằng một node mới ngay lập tức . Các nhân chứng được trả một khoản phí để tạo ra các khối. Phí do những người staking quy định.

>Thông thường tất cả các node tạo ra các khối tại một thời điểm theo kiểu vòng tròn. Điều này ngăn một node xuất bản các khối liên tiếp, ngăn anh ta thực hiện các cuộc tấn công [double-spending](https://cryptoviet.com/double-spending-la-gi). Nếu một nhân chứng không tạo ra một khối trong khe thời gian của họ, thì khoảng thời gian đó sẽ bị bỏ qua và nhân chứng tiếp theo tạo ra khối tiếp theo. Nếu một nhân chứng liên tục bỏ lỡ các khối của anh ta hoặc công bố các giao dịch không hợp lệ thì những người đặt cược sẽ bỏ phiếu cho anh ta và thay thế anh ta bằng một nhân chứng tốt hơn.

>Trong DPoS, miners có thể cộng tác để tạo ra các khối thay vì cạnh tranh như trong PoW và PoS. Bằng cách tập trung một phần vào việc tạo ra các khối, DPoS có thể chạy các lệnh có quy mô nhanh hơn hầu hết các thuật toán đồng thuận khác. EOS (sử dụng dPoS) là blockchain đầu tiên đạt được thời gian khối là 0,5 giây !.
Nhanh thật.

5. Proof-of-Authority (Bằng chứng về thẩm quyền)
![PoA](https://affidaty.io/blog/wp-content/uploads/2019/08/POA-ENG-1-768x520.jpg)
- Ưu điểm:
    - Tiết kiệm năng lượng.
    - Nhanh.
- Nhược điểm:
    - Một chút tập trung. 
    - Có thể được sử dụng trong các chuỗi khối công khai nhưng thường được sử dụng trong các chuỗi khối riêng tư, được cấp phép.
- Được sử dụng bởi: POA.Network, Ethereum Kovan testnet, VeChain
- Loại: Đồng thuận hợp tác
- Giải thích: 
Trong các mạng dựa trên PoA, các giao dịch và khối được xác thực bởi các tài khoản được phê duyệt, được gọi là trình xác thực. Trình xác thực chạy phần mềm cho phép họ đưa các giao dịch vào các khối. Quá trình này được tự động hóa và không yêu cầu người xác nhận phải liên tục giám sát máy tính của họ. Tuy nhiên, nó yêu cầu duy trì máy tính (node quyền hạn) không bị xâm phạm.

Ba điều kiện chính phải được đáp ứng để thiết lập trình xác nhận là:
>- Danh tính phải được xác minh chính thức trên chuỗi, với khả năng kiểm tra chéo thông tin trong một miền có sẵn công khai
>- Tính đủ điều kiện phải khó đạt được, để có quyền xác nhận các khối kiếm được và có giá trị. (Ví dụ: người xác nhận tiềm năng được yêu cầu phải có giấy phép công chứng)
>- Phải có sự thống nhất hoàn toàn trong việc kiểm tra và thủ tục để thiết lập một cơ quan có thẩm quyền

Với PoA, các cá nhân có quyền trở thành validator, do đó, có động cơ để duy trì vị trí mà họ đã đạt được. Bằng cách gắn danh tiếng với danh tính, người xác thực được khuyến khích duy trì quy trình giao dịch, vì họ không muốn danh tính của mình gắn liền với danh tiếng tiêu cực, do đó mất vai trò người xác thực khó kiếm được.

6. Proof-of-Weight(Bằng chứng về trọng lượng)

![PoWeight](https://cryptomaniaks.com/sites/default/files/pictures/proof-of-weight-compressed.gif)

- Ưu điểm:
    - Tiết kiệm năng lượng.
    - Có thể tùy chỉnh cao và có thể mở rộng.
- Nhược điểm:
    - Khuyến khích có thể khó.
- Được sử dụng bởi: Algorand
- Loại: Đồng thuận cạnh tranh
- Giải thích: 
>Proof-of-Weight là một phân loại rộng rãi của các thuật toán đồng thuận dựa trên mô hình đồng thuận Algorand. Ý tưởng chung là trong PoS, tỷ lệ phần trăm mã thông báo sở hữu trong mạng của bạn thể hiện xác suất "discovering-khám phá" khối tiếp theo của bạn, trong hệ thống PoWeight, một số giá trị tương đối có trọng số khác được sử dụng. Một số triển khai của nó là Proof of Reputation và Proof of Space.


7. Proof of Reputation(Bằng chứng về danh tiếng)

- Ưu điểm:
    - Tốt cho các mạng riêng tư, được phép.
- Nhược điểm:
    - Chỉ được sử dụng trong các blockchain riêng tư, được cấp phép.
- Được sử dụng bởi: GoChain
- Loại: Đồng thuận hợp tác
- [Giải thích](https://arxiv.org/pdf/1806.07342.pdf): 
>Tương tự như Proof of Authority. Như GoChain đã đề cập:
Mô hình đồng thuận Proof of Reputation (PoR) phụ thuộc vào danh tiếng của những người tham gia để giữ an toàn cho mạng. Một người tham gia (a block signer-người ký khối) phải có danh tiếng đủ quan trọng để họ phải đối mặt với những hậu quả đáng kể về tài chính và thương hiệu nếu họ cố gắng gian lận hệ thống. Đây là một khái niệm tương đối vì hầu như tất cả các doanh nghiệp sẽ bị thiệt hại đáng kể nếu họ bị bắt quả tang cố gắng gian dối, nhưng các công ty lớn hơn thường sẽ có nhiều thứ để mất hơn và do đó được lựa chọn hơn các công ty ít sử dụng hơn (các doanh nghiệp nhỏ hơn).
Khi một công ty chứng minh được danh tiếng và vượt qua xác minh, họ có thể được bình chọn vào mạng như một node có thẩm quyền và tại thời điểm này, nó hoạt động giống như mạng Bằng chứng về quyền (PoA), nơi chỉ các node có thẩm quyền mới có thể ký và xác nhận các khối.


8. Proof of Elapsed Time (Bằng chứng về thời gian đã trôi qua)
- Ưu điểm:
    - Chi phí tham gia thấp, do đó nhiều người hơn có thể tham gia dễ dàng, do đó được phân cấp.
    - Thật đơn giản cho tất cả những người tham gia để xác minh rằng người lãnh đạo đã được lựa chọn một cách hợp pháp.
    - Chi phí cho việc kiểm soát quá trình bầu cử lãnh đạo tỷ lệ thuận với giá trị thu được từ nó.
- Nhược điểm:
    - Mặc dù nó rẻ nhưng bạn phải sử dụng phần cứng chuyên dụng. Do đó không thể được áp dụng đại trà.
    - Không phù hợp với các blockchain công khai.
- Được sử dụng bởi: HyperLedger Sawtooth
- Loại: Đồng thuận cạnh tranh
- Giải thích: 
>PoET là một thuật toán cơ chế đồng thuận thường được sử dụng trên các mạng blockchain được cấp phép để quyết định quyền khai thác hoặc người chiến thắng khối trên mạng. Các mạng blockchain được phép là những mạng yêu cầu bất kỳ người tham gia tiềm năng nào phải xác định danh tính bản thân trước khi họ được phép tham gia. Dựa trên nguyên tắc của một hệ thống xổ số công bằng trong đó mọi node đơn lẻ đều có khả năng là người chiến thắng như nhau, cơ chế PoET dựa trên việc phân chia cơ hội chiến thắng một cách công bằng cho số lượng người tham gia mạng lớn nhất có thể.

>Hoạt động của thuật toán PoET như sau. Mỗi node tham gia trong mạng được yêu cầu đợi trong một khoảng thời gian được chọn ngẫu nhiên và node đầu tiên hoàn thành thời gian chờ được chỉ định sẽ thắng khối mới. Mỗi node trong mạng blockchain tạo ra thời gian chờ ngẫu nhiên và chuyển sang chế độ ngủ trong khoảng thời gian được chỉ định đó. Người thức dậy đầu tiên - tức là người có thời gian chờ ngắn nhất - thức dậy và cam kết một khối mới cho blockchain, phát thông tin cần thiết cho toàn bộ mạng ngang hàng. Quá trình tương tự sau đó lặp lại để phát hiện ra khối tiếp theo.

>Cơ chế đồng thuận của mạng PoET cần đảm bảo hai yếu tố quan trọng. Đầu tiên, các node tham gia thực sự chọn thời gian thực sự là ngẫu nhiên và không phải là khoảng thời gian ngắn hơn do những người tham gia cố ý chọn để giành chiến thắng. Hai là người chiến thắng đã thực sự hoàn thành thời gian chờ đợi.

>Cơ chế sâu sắc cho phép các ứng dụng thực thi mã đáng tin cậy trong một môi trường được bảo vệ và điều này đảm bảo rằng cả hai yêu cầu - để chọn ngẫu nhiên thời gian chờ cho tất cả các node tham gia và hoàn thành thực sự thời gian chờ của người tham gia chiến thắng - đều được đáp ứng.

>Cơ chế chạy mã tin cậy trong một môi trường an toàn cũng quan tâm đến nhiều nhu cầu thiết yếu khác của mạng. Nó đảm bảo rằng mã đáng tin cậy thực sự chạy trong môi trường an toàn và không thể thay đổi bởi bất kỳ người tham gia bên ngoài nào. Nó cũng đảm bảo rằng các kết quả có thể được xác minh bởi những người tham gia và thực thể bên ngoài, do đó nâng cao tính minh bạch của sự đồng thuận của mạng lưới.

>PoET kiểm soát chi phí của quy trình đồng thuận và giữ cho nó nhanh nhẹn để chi phí vẫn tỷ lệ thuận với giá trị thu được từ quy trình, một yêu cầu quan trọng để nền kinh tế tiền điện tử tiếp tục phát triển.

9. Proof-of-space (PoSpace) hay còn gọi là proof-of-capacity (PoC)
![PoC](https://miro.medium.com/max/1072/0*cTn0KjZxAS1NUmBe.jpg)
- Ưu điểm:
    - Tương tự như PoW nhưng sử dụng không gian thay vì tính toán. Do đó rất thân thiện với môi trường.
    - Có thể được sử dụng để phát hiện phần mềm độc hại, bằng cách xác định xem bộ nhớ đệm L1 của bộ xử lý có trống không (ví dụ: có đủ dung lượng để đánh giá quy trình PoSpace mà không bỏ sót bộ nhớ cache) hay chứa một quy trình chống lại việc bị loại bỏ.
    - Có thể được sử dụng cho các biện pháp chống thư rác và phòng chống tấn công từ chối dịch vụ.
- Nhược điểm:
    - Incentivization
- Được sử dụng bởi: Burstcoin, Chia, SpaceMint
- Loại: Đồng thuận hợp tác
- Giải thích: 
>Proof-of-space (PoSpace), còn được gọi là bằng chứng về dung lượng (PoC), là một phương tiện thể hiện rằng một người có lợi ích hợp pháp đối với một dịch vụ (chẳng hạn như gửi email) bằng cách phân bổ một số tiền không nhỏ bộ nhớ hoặc dung lượng đĩa để giải quyết một thách thức do nhà cung cấp dịch vụ đưa ra. Khái niệm này được xây dựng bởi Dziembowski và cộng sự. vào năm 2015. (Bài báo của Ateniese và cộng sự, đồng thời có tiêu đề Proof-of-space, trên thực tế là một giao thức Proof-of-work khó có bộ nhớ).

>Bằng chứng về không gian rất giống với bằng chứng về công việc, ngoại trừ việc thay vì tính toán, lưu trữ được sử dụng. Proof-of-space có liên quan đến, nhưng cũng khác đáng kể với, các chức năng khó có bộ nhớ và các bằng chứng về khả năng truy xuất.

>Bằng chứng về không gian là một phần dữ liệu mà một câu tục ngữ gửi đến một người xác minh để chứng minh rằng câu tục ngữ đã dành một khoảng không gian nhất định. Để thực tế, quy trình xác minh cần phải hiệu quả, cụ thể là tiêu tốn một lượng nhỏ không gian và thời gian. Đối với tính hợp lý, câu tục ngữ sẽ khó có thể vượt qua xác minh nếu nó không thực sự dành đủ dung lượng đã được xác nhận. Một cách để triển khai PoSpace là sử dụng các đồ thị khó làm bằng đá cuội. Người xác minh yêu cầu câu châm ngôn xây dựng nhãn hiệu của một đồ thị khó có thể cắt được. Câu tục ngữ cam kết về việc dán nhãn. Người xác minh sau đó yêu cầu người châm ngôn mở một số vị trí ngẫu nhiên trong cam kết.

>Bằng chứng về không gian được coi là một giải pháp thay thế xanh hơn và công bằng hơn do tính chất mục đích chung của lưu trữ và chi phí năng lượng thấp hơn yêu cầu của lưu trữ.   

10. Proof of History(Bằng chứng lịch sử)



![PoH](https://www.mobileappdaily.com/public/uploads/mad_11239cd59a5.png)

*Proof of History Timestamps*

- Được sử dụng bởi: Solana
- Giải thích: 
>Ý tưởng cơ bản ở đây là thay vì tin tưởng vào dấu thời gian trên giao dịch, bạn có thể chứng minh rằng giao dịch đó đã xảy ra trước và sau một sự kiện.

>Khi bạn chụp một bức ảnh với trang bìa của New York Times, bạn đang tạo ra một bằng chứng rằng bức ảnh của bạn được chụp sau khi tờ báo đó được xuất bản, hoặc bạn có một số cách để ảnh hưởng đến những gì New York Times xuất bản. Với Proof of History, bạn có thể tạo một bản ghi lịch sử chứng minh rằng một sự kiện đã xảy ra tại một thời điểm cụ thể.

<b>Dấu thời gian bằng chứng về lịch sử</b>

>Bằng chứng lịch sử là một chức năng trì hoãn có thể xác minh được tần số cao. Chức năng Độ trễ có thể xác minh được yêu cầu một số bước tuần tự cụ thể để đánh giá, nhưng vẫn tạo ra một đầu ra duy nhất có thể được xác minh một cách hiệu quả và công khai.
Việc triển khai cụ thể này sử dụng một hàm băm kháng trước hình ảnh tuần tự chạy qua chính nó liên tục với đầu ra trước đó được sử dụng làm đầu vào tiếp theo. Định kỳ số đếm và đầu ra hiện tại được ghi lại.

>Đối với hàm băm SHA256, quá trình này không thể song song mà không có cuộc tấn công bạo lực sử dụng 2¹²⁸ lõi.
Sau đó, chúng ta có thể chắc chắn rằng thời gian thực đã trôi qua giữa mỗi bộ đếm khi nó được tạo và thứ tự được ghi lại của mỗi bộ đếm giống như trong thời gian thực.

11. Proof of Stake Velocity

- Được sử dụng bởi: Reddcoin
- Giải thích: 
>Proof of Stake Velocity (PoSV) được đề xuất thay thế cho Proof of Work (PoW) và Proof of Stake (PoS) để bảo mật mạng ngang hàng và xác nhận các giao dịch của Reddcoin, một loại tiền điện tử được tạo ra đặc biệt để tạo điều kiện cho xã hội tương tác trong thời đại kỹ thuật số. PoSV được thiết kế để khuyến khích cả quyền sở hữu (Cổ phần) và hoạt động (Vận tốc) tương ứng trực tiếp với hai chức năng chính của Reddcoin như một loại tiền tệ thực: lưu trữ giá trị và phương tiện trao đổi. Reddcoin cũng có thể hoạt động như một đơn vị tài khoản trong bối cảnh xã hội không đồng nhất.

12. Proof of Importance (Bằng chứng về tầm quan trọng)
![PoI](https://www.btcwires.com/wp-content/uploads/Why_Proof_of_Importance-01.png)
- Ưu điểm:
    - Tốt hơn PoS trong việc đánh giá cổ phần.
- Được sử dụng bởi: NEM
- Giải thích: 
>Mạng lưới đồng thuận của NEM không chỉ phụ thuộc vào số lượng tiền xu mà còn phụ thuộc vào khả năng hoạt động của hệ thống hiệu quả sẽ được trả công. Cơ hội đặt cược một khối là một thành phần của nhiều yếu tố khác nhau, bao gồm danh tiếng (được kiểm soát bởi một khuôn khổ được thiết kế cho mục đích khác), số dư và số lượng giao dịch được thực hiện đến và đi từ vị trí đó. Đây được gọi là tính toán mức độ quan trọng. Điều này mang lại hình ảnh toàn diện hơn về thành viên hệ thống 'hữu ích'.

>Để đủ điều kiện cho phép tính mức độ quan trọng, người dùng cần có ít nhất 10.000 XEM trong số dư của họ. Xem xét chỉ có dưới 9 tỷ XEM đang lưu hành, việc đạt được mục tiêu đó không phải là quá tốn kém. Có thể ngưỡng 10.000 XEM này sẽ bị thay đổi trong tương lai, nhưng hiện tại, nó vẫn vậy. Nhưng việc tính toán mức độ quan trọng được thực hiện bằng cách sử dụng một thuật toán cụ thể, không chỉ bằng xác suất và kích thước cổ phiếu của chúng.

>Điều quan trọng cần lưu ý là bằng chứng tầm quan trọng của NEM có khả năng chống lại việc thao túng tùy tiện. Các cuộc tấn công Sybil và các cuộc tấn công vòng lặp được giảm thiểu bằng cách sử dụng các cơ chế cơ bản của sự đồng thuận. Điều quan trọng không kém cần nhớ là bằng chứng về tầm quan trọng không phải là bằng chứng về tiền đặt cọc, mặc dù rất dễ để rút ra sự tương đồng giữa hai điều này.

13. Proof of Burn
![PoB](https://miro.medium.com/max/1204/1*4ze-9kcQOoFuWFamjxjtRQ.png)
- Được sử dụng bởi: Slimcoin, TGCoin
- Giải thích: 
>Với Proof of Burn, thay vì đổ tiền vào thiết bị máy tính đắt tiền, bạn 'đốt' tiền bằng cách gửi chúng đến một địa chỉ mà chúng không thể thu hồi được. Bằng cách cam kết đồng tiền của bạn không bao giờ được trả lại, bạn kiếm được đặc quyền suốt đời để khai thác trên hệ thống dựa trên quy trình lựa chọn ngẫu nhiên.
Tùy thuộc vào cách triển khai bằng chứng ghi, các thợ đào có thể đốt coin trên chuỗi chính hoặc coin của một chuỗi thay thế, chẳng hạn như bitcoin. Bạn đốt càng nhiều tiền, bạn càng có cơ hội được chọn để khai thác khối tiếp theo.
Theo thời gian, tiền đặt cược của bạn trong hệ thống giảm dần, vì vậy cuối cùng bạn sẽ muốn đốt thêm tiền để tăng tỷ lệ được chọn trong xổ số. (Điều này bắt chước quy trình khai thác của bitcoin, nơi bạn phải liên tục đầu tư vào thiết bị máy tính hiện đại hơn để duy trì sức mạnh hàm băm.)
Mặc dù bằng chứng ghi là một sự thay thế thú vị cho bằng chứng công việc, nhưng giao thức này vẫn lãng phí tài nguyên một cách không cần thiết. Một lời chỉ trích khác là sức mạnh khai thác chỉ đơn giản đến với những người sẵn sàng đốt nhiều tiền hơn.

14. Proof of Identity

- Giải thích: Bằng chứng nhận dạng (PoI) là bằng chứng mật mã (phần dữ liệu) cho biết rằng bất kỳ người dùng nào cũng biết khóa riêng tư so với danh tính được ủy quyền và được gắn bằng mật mã vào một giao dịch cụ thể. Mọi cá nhân từ một số nhóm có thể tạo PoF (chỉ một khối dữ liệu) và trình bày nó cho bất kỳ ai, chẳng hạn như node xử lý.


15. Proof Of Activity

![PoA](https://miro.medium.com/max/1838/1*jWlGrYH-TqHZ201pyj7gxw.png)

- Được sử dụng bởi: Decred
- Giải thích: 

>Để tránh lạm phát phi mã (điều gì xảy ra khi quá nhiều tiền tệ làm ngập hệ thống) bitcoin sẽ chỉ tạo ra 21 triệu bitcoin. Điều đó có nghĩa là, tại một thời điểm nào đó, trợ cấp phần thưởng khối bitcoin sẽ kết thúc và những người khai thác bitcoin sẽ chỉ nhận được phí giao dịch.

>Trong bằng chứng hoạt động, khai thác bắt đầu theo kiểu bằng chứng công việc truyền thống, với các thợ đào chạy đua để giải một câu đố mật mã. Tùy thuộc vào việc triển khai, các khối được khai thác không chứa bất kỳ giao dịch nào (chúng giống với các mẫu hơn), do đó, khối chiến thắng sẽ chỉ chứa tiêu đề và địa chỉ phần thưởng của người khai thác.

>Tại thời điểm này, hệ thống chuyển sang bằng chứng cổ phần. Dựa trên thông tin trong tiêu đề, một nhóm trình xác nhận ngẫu nhiên được chọn để ký vào khối mới. Người xác thực sở hữu càng nhiều tiền trong hệ thống, thì người đó càng có nhiều khả năng được chọn. Mẫu trở thành một khối chính thức ngay sau khi tất cả các trình xác thực ký tên vào nó.

>Nếu một số trình xác thực đã chọn không có sẵn để hoàn thành khối, thì khối chiến thắng tiếp theo sẽ được chọn, một nhóm trình xác nhận mới sẽ được chọn, v.v. cho đến khi một khối nhận được số lượng chữ ký chính xác. Phí được phân chia giữa người khai thác và người xác nhận đã ký vào khối.

>Các chỉ trích về bằng chứng hoạt động cũng giống như đối với cả bằng chứng về công việc (cần quá nhiều năng lượng để khai thác các khối) và bằng chứng về cổ phần (không có gì để ngăn cản người xác nhận ký hai lần).


16. Proof of Time
![PoT]()
- Được sử dụng bởi: Chronologic

- Giải thích: 
>Bằng chứng về thời gian được giới thiệu bởi Chronologic. Họ đang có kế hoạch xây dựng một blockchain riêng biệt. Như đã nêu bởi nhà phát triển chính của họ:
Vấn đề ở đây là số lượng lớn nhất có thể được lưu trữ trong một biến ở độ vững chắc có độ lớn là 1076. Điều này gây khó khăn cho chúng tôi khi làm việc với thời gian và việc tạo ra các mã thông báo.

17. Proof of Existence

![PoE](https://miro.medium.com/max/1400/1*8HriYqKzC1X5ebJXUH-9bA.png)

- Bằng chứng về sự tồn tại
- Được sử dụng bởi: Poex.io, HeroNode, DragonChain
- Giải thích: 
>Proof of Existence là một dịch vụ trực tuyến xác minh sự tồn tại của các tệp máy tính tại một thời điểm cụ thể thông qua các giao dịch được đánh dấu thời gian trong chuỗi khối bitcoin.
Nó được đưa ra vào năm 2013 dưới dạng một dự án mã nguồn mở. Nó được phát triển bởi Manuel Araoz và Esteban Ordano.
- Trường hợp sử dụng:
    - Thỏa thuận ký số mà không tiết lộ nội dung thực tế.
    - Chứng minh quyền sở hữu dữ liệu mà không tiết lộ dữ liệu thực tế.
    - Thời gian đóng dấu tài liệu.
    - Chứng minh quyền sở hữu

18. Proof of Retrievability
![PoR](https://static-01.hindawi.com/articles/wcmc/volume-2018/4186243/figures/4186243.fig.001.svgz)
- Được sử dụng bởi: Microsoft
- Giải thích: 
>Bằng chứng về khả năng truy xuất (POR) là một bằng chứng nhỏ gọn của hệ thống tệp (phương thức) đối với máy khách (người xác minh) rằng tệp đích F là nguyên vẹn, theo nghĩa là máy khách có thể khôi phục hoàn toàn. Vì POR có độ phức tạp truyền thông thấp hơn so với truyền của chính F, chúng là một khối xây dựng hấp dẫn cho các hệ thống lưu trữ từ xa có độ đảm bảo cao. Nó có thể thực sự hữu ích như một thuật toán đồng thuận cho các hệ thống Điện toán đám mây.

19. Proof of Believability(Bằng chứng về độ tin cậy)
![PoB](https://miro.medium.com/max/1838/0*OZdTXa6OiM-9nq98)
- Ưu điểm:
    - Phân cấp hơn PoS truyền thống đó bằng cách sử dụng khái niệm Servi.
    - Kết thúc nhanh so với PoS truyền thống.
- Được sử dụng bởi: IOST
- Giải thích: 
    
    Một thách thức lớn mà cơ chế đồng thuận Proof-of-Stake truyền thống phải đối mặt là xu hướng tập trung hóa. Để giảm thiểu rủi ro này, IOST đã giới thiệu Servi vừa là thước đo mức độ đóng góp của người dùng cho cộng đồng vừa là một cách để khuyến khích các thành viên đóng góp vào sự phát triển liên tục của IOSChain. Nó có các thuộc tính sau:
    - <b>Không thể giao dịch</b>: Vì Servi không được thiết kế như một phương tiện trao đổi, Servi không thể được mua bán hoặc trao đổi dưới bất kỳ hình thức nào.
    - <b>Tự hủy</b>: Sau khi xác thực một khối, hệ thống sẽ tự động xóa số dư Servi do người xác thực sở hữu. Bằng cách này, các node có điểm đáng tin cậy cao có thể thay phiên nhau xác nhận các khối, để đảm bảo quá trình tạo khối công bằng.
    - <b>Tự phát hành</b>: Servi sẽ tự động được tạo và gửi vào tài khoản người dùng sau một số đóng góp nhất định, chẳng hạn như cung cấp dịch vụ cộng đồng, đánh giá dịch vụ do một tổ chức khác cung cấp và / hoặc đóng góp đặc biệt khác.

    Các hệ thống blockchain truyền thống có sự đánh đổi cố hữu giữa an toàn và thông lượng, tùy thuộc vào kích thước phân đoạn. Một hệ thống với số lượng lớn các phân đoạn nhỏ mang lại hiệu suất tốt hơn nhưng cung cấp khả năng phục hồi kém hơn trước các tác nhân xấu và ngược lại (Một trong những vấn đề mà Casper cũng phải đối mặt). Để phá vỡ sự đánh đổi theo cách giữ an toàn và tăng thông lượng, IOST đã đề xuất một giao thức đồng thuận Proof-of-Believability (PoB) sáng tạo cho IOSChain. PoB đảm bảo rằng các node có xác suất hoạt động sai không đáng kể, đồng thời tăng đáng kể thông lượng giao dịch theo kích thước-một-phân đoạn.

    Giao thức đồng thuận Proof-of-Believability sử dụng phương pháp tiếp cận Tin tưởng - Đầu tiên trong phân đoạn. Giao thức chia tất cả các trình xác nhận thành hai nhóm, một liên minh đáng tin cậy và một liên minh bình thường. Trình xác thực đáng tin cậy xử lý giao dịch nhanh chóng trong giai đoạn đầu tiên. Sau đó, trình xác thực thông thường lấy mẫu và xác minh các giao dịch trong giai đoạn thứ hai để cung cấp tính chính xác và đảm bảo khả năng xác minh. Cơ hội để một node được bầu chọn vào giải đấu đáng tin cậy được xác định bằng điểm đáng tin cậy được tính bằng nhiều yếu tố (ví dụ: số dư mã thông báo, đóng góp cho cộng đồng, đánh giá, v.v.). Một người có điểm số đáng tin cậy cao hơn có nhiều khả năng được bầu vào giải đấu đáng tin cậy hơn. Người xác nhận đáng tin cậy tuân theo các thủ tục để quyết định tập hợp các giao dịch đã cam kết và thứ tự của chúng, cũng như xử lý chúng theo thứ tự. Trình xác thực đáng tin cậy cũng tạo thành các nhóm nhỏ hơn - một trình xác nhận cho mỗi nhóm. Các giao dịch sẽ được phân phối ngẫu nhiên giữa các trình xác thực đáng tin cậy này. Do đó, chúng tạo ra các khối nhỏ hơn với độ trễ cực thấp.
    Tuy nhiên, nó có thể gây ra vấn đề bảo mật vì chỉ có một node đang thực hiện xác minh. Do đó, một số giao dịch bị hỏng có thể được thực hiện bởi các trình xác thực hoạt động sai. Để giải quyết vấn đề bảo mật này, họ chỉ định xác suất lấy mẫu mà các trình xác nhận thông thường sẽ lấy mẫu các giao dịch và phát hiện sự không nhất quán. Nếu trình xác thực bị phát hiện là hành vi sai, nó sẽ mất tất cả các mã thông báo và danh tiếng trong hệ thống trong khi những người dùng bị lừa đảo sẽ được bồi thường cho bất kỳ tổn thất nào. Phương pháp đầu tiên đáng tin cậy làm cho việc xử lý các giao dịch cực kỳ nhanh chóng vì chỉ có một trình xác thực (đáng tin cậy) duy nhất đang thực hiện xác minh và nó không có khả năng hoạt động sai.