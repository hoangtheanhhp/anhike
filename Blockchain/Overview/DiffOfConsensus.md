# Các thuật toán đồng thuận: Gốc rễ của công nghệ blockchain 

Chúng ta đã nghe rất nhiều rằng Blockchain sẽ là cuộc cách mạng thay đổi nền kinh tế toàn cầu vì các ưu điểm như tốc độ, sụ minh bạch, bảo mật. Điều đem lại những ưu điểm trên cho blockchain chính là các thuật toán đồng thuận trong đó. Quả không sai khi nói thuật toán đồng thuận là gốc rễ của công nghệ mới này.

Các thuật toán đồng thuận trong blockchain là những gì làm cho tất cả các chuỗi đồng thuận blockchain khác với nhau. Mạng lưới chuỗi khối có hàng triệu triệu người trong cùng một không gian. Vì vậy, tại sao chúng không bao giờ can thiệp lẫn nhau hoặc tồn tại lẫn nhau?

Câu trả lời là trong kiến trúc của mạng blockchain. Kiến trúc được thiết kế thông minh và các thuật toán đồng thuận là cốt lõi của kiến trúc này.

## Thuật toán đồng thuận

Các thuật toán đồng thuận là một quá trình ra quyết định cho một nhóm, nơi các cá nhân trong nhóm xây dựng và hỗ trợ quyết định phù hợp nhất với những người còn lại. Đó là một hình thức giải quyết mà các cá nhân cần ủng hộ quyết định của đa số, cho dù họ có thích hay không.

Nói một cách dễ hiểu, đó chỉ là một phương pháp để quyết định trong một nhóm. Hãy để tôi làm rõ nó với một ví dụ. Hãy tưởng tượng một nhóm mười người muốn đưa ra quyết định về một dự án có lợi cho tất cả họ. Mỗi người trong số họ có thể đề xuất một ý tưởng, nhưng đa số sẽ ủng hộ ý tưởng giúp họ nhiều nhất. Những người khác phải đối phó với quyết định này cho dù họ muốn hay không.

Bây giờ hãy tưởng tượng điều tương tự với hàng ngàn người. Điều đó sẽ không làm cho nó trở nên khó khăn hơn sao?

Các thuật toán đồng thuận không chỉ đồng ý với đa số phiếu bầu, mà còn đồng ý với một thuật toán có lợi cho tất cả họ. Vì vậy, mạng luôn có lợi.

![image](https://101blockchains.com/wp-content/uploads/2018/08/Different_Consensus_Algorithms.png)

## Sự khác nhau giữa các thuật toán đồng thuận 
List of All Consensus Algorithms
Proof-of-Work
Proof-of-Stake
Delegated Proof-of-Stake
Leased Proof-Of-Stake
Proof of Elapsed Time
Practical Byzantine Fault Tolerance
Simplified Byzantine Fault Tolerance
Delegated Byzantine Fault Tolerance
Directed Acyclic Graphs
Proof-of-Activity
Proof-of-Importance
Proof-of-Capacity
Proof-of-Burn
Proof-of-Weight



## Các thuật toán đồng thuận khác
Bằng chứng hoạt động
Trong khi mọi người đang tranh luận về chủ đề - Proof-of-Work so với Proof-of-Stake, người tạo ra Litecoin và ba tác giả khác đã nghĩ ra một thứ gì đó tuyệt vời. Họ đã hỏi thế giới một câu hỏi đơn giản - tại sao không thể kết hợp PoW và PoS thay vì khiến chúng chiến đấu với nhau?

Vì vậy, ý tưởng về một sự lai tạo hấp dẫn đã xuất hiện trên thế giới - Proof-of-Activity. Nó kết hợp hai tính năng tốt nhất - bảo mật hơn trước mọi cuộc tấn công và không phải là một hệ thống không ngốn điện.

Bằng chứng hoạt động hoạt động như thế nào?

Trong giao thức đồng thuận blockchain Proof-of-Activity, quá trình khai thác bắt đầu giống như thuật toán PoW. Các thợ mỏ giải một câu đố quan trọng để nhận phần thưởng. Vì vậy, đâu là sự khác biệt quan trọng với PoW? Trong PoW, thợ đào khai thác các khối có giao dịch hoàn chỉnh.

Trong Proof-of-Activity, người khai thác chỉ khai thác mẫu của các khối. Một mẫu như vậy có hai thứ - thông tin tiêu đề và địa chỉ phần thưởng cho các thợ đào.

Một khi, các thợ đào khai thác các mẫu khối này; hệ thống chuyển đổi sang Proof-of-Stakes. Thông tin tiêu đề bên trong một khối trỏ đến một bên liên quan ngẫu nhiên. Các bên liên quan này sau đó xác nhận các khối được khai thác trước.

Trình xác thực càng giữ nhiều ngăn xếp, thì khả năng họ chấp thuận một khối càng tăng. Chỉ sau khi xác thực, khối cụ thể đó mới được đưa vào blockchain.

Đây là cách Proof-of-Activity sử dụng tốt nhất trong số hai thuật toán đồng thuận để xác thực và thêm một khối vào blockchain. Hơn nữa, mạng lưới trả cho cả người khai thác và người xác nhận phần chi phí giao dịch hợp lý. Do đó, hệ thống hành động chống lại "thảm kịch của các điểm chung" và tạo ra một giải pháp tốt hơn để xác nhận khối.

Các tác động của Proof-of-Activity

Một trong những mối đe dọa lớn nhất mà blockchain phải đối mặt là cuộc tấn công 51%. Định lý đồng thuận làm giảm xác suất của cuộc tấn công 51% xuống 0. Nó xảy ra vì cả người khai thác và người xác nhận đều không thể chiếm đa số vì quá trình sẽ yêu cầu đóng góp như nhau trong khi thêm một khối vào mạng.

Mặc dù, một số nhà phê bình nói rằng giao thức đồng thuận blockchain Proof-of-Activity có một số sai sót nghiêm trọng. Điều đầu tiên sẽ là mức tiêu thụ năng lượng lớn do tính năng khai thác. Thứ hai, Proof-of-Activity không có bất kỳ giải pháp nào để ngăn chặn việc ký hai lần của những người xác thực. Hai sai sót đáng kể này làm cho định lý đồng thuận bị lùi lại một chút.

Hai blockchain phổ biến áp dụng Proof-of-Activity - Decred và Espers. Tuy nhiên, chúng có một số biến thể. Trên thực tế, Decred đang được coi là định lý phổ biến hơn cả định lý đồng thuận Espers.

Bằng chứng tầm quan trọng

Tiếp theo trong danh sách của chúng tôi là giao thức đồng thuận blockchain Proof-of-Importance. Ví dụ về sự đồng thuận này xuất hiện là do cái tên nổi tiếng của NEM. Khái niệm này là sự phát triển của Proof-of-Stake. Mặc dù, NEM đã đưa ra một ý tưởng mới - thu hoạch hoặc thu hoạch.

Cơ chế thu hoạch xác định xem một nút có đủ điều kiện để được thêm vào blockchain hay không. Bạn càng thu hoạch được nhiều trên một nút, thì càng có nhiều cơ hội được thêm vào chuỗi. Đổi lại cho việc thu hoạch, nút nhận được phí giao dịch mà trình xác nhận thu được làm phần thưởng. Để đủ điều kiện thu hoạch, bạn cần có ít nhất 10.000 XEM trong tài khoản của mình.

Nó giải quyết vấn đề chính của Proof-of-Stake. Trong PoS, người giàu nhận được nhiều tiền hơn so với người xác nhận có ít tiền hơn. Ví dụ: nếu bạn sở hữu 20% tiền điện tử, bạn có thể khai thác 20% tất cả các khối trên mạng blockchain. Điều này làm cho các thuật toán đồng thuận thuận lợi cho những người giàu có.

Đặc điểm đáng chú ý của Bằng chứng tầm quan trọng

Vesting
Đặc điểm hấp dẫn nhất của định lý đồng thuận là sự tranh giành hoặc thu hoạch. Như chúng tôi đã nói, bạn cần có ít nhất 10.000 xu để đủ điều kiện thu hoạch ngay từ đầu. Điểm Chứng minh Tầm quan trọng của bạn phụ thuộc vào số tiền thu hoạch được mà bạn có. Mặc dù, các thuật toán đồng thuận có tính đến khoảng thời gian bạn có tiền trong túi.

Quan hệ đối tác giao dịch
Thuật toán Bằng chứng tầm quan trọng sẽ thưởng cho bạn nếu bạn thực hiện giao dịch với các chủ tài khoản NEM khác. Mạng sẽ coi hai bạn là đối tác. Mặc dù vậy, hệ thống sẽ bắt bạn nếu bạn đang có ý định tạo quan hệ đối tác giả.

Hệ thống tính điểm
Các giao dịch có ảnh hưởng đến điểm Bằng chứng quan trọng của bạn. Điểm số dựa trên các giao dịch bạn đã thực hiện trong khoảng thời gian ba mươi ngày. Số tiền thường xuyên hơn và đáng kể hơn sẽ giúp bạn cải thiện điểm số của mình trên mạng NEM.

Bằng chứng năng lực

Ví dụ về sự đồng thuận bằng chứng về năng lực là một bản nâng cấp của giao thức đồng thuận blockchain Proof-of-Work nổi tiếng. Đặc điểm cơ bản của cái này là tính năng "âm mưu". Bạn sẽ phải dành sức mạnh tính toán và bộ nhớ ổ cứng của mình ngay cả trước khi bạn bắt đầu khai thác.

Chính bản chất này làm cho hệ thống nhanh hơn PoW. Proof-of-Capacity có thể tạo một khối chỉ trong bốn phút trong khi Proof-of-Work mất mười phút để làm điều tương tự. Hơn nữa, nó