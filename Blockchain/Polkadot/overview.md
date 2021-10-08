#　4.3　Consensus

Trong phần này, chúng tôi giải thích giao thức đồng thuận kết hợp của Polkadot bao gồm BABE: một
cơ chế tạo block của relay chain - cung cấp xác suất cuối cùng và GRANDPA
cung cấp tính cuối cùng có thể chứng minh, xác định được và hoạt động độc lập với BABE.
Không chính thức tính cuối cùng theo xác suất ngụ ý rằng sau khi thời gian nhất định trôi qua, một khối trong relay chain sẽ được hoàn thiện
với xác suất rất cao (gần bằng 1) và tính xác định cuối ngụ ý rằng một khối đã hoàn thành vẫn là khối cuối cùng
mãi mãi. Hơn nữa, tính chứng minh cuối cùng có nghĩa là chúng tôi có thể chứng minh cho các bên không tham gia tích cực vào
sự đồng thuận rằng một khối là cuối cùng.

Chúng tôi cần tính chứng minh sau cùng để tạo cầu nối với các chuỗi bên ngoài Polkadot dễ dàng hơn(một blockchain khác-
không nằm trong cơ chế đồng thuận của Polkadot sau đó có thể được thuyết phục về thời điểm an toàn để hành động trên dữ liệu trong một relay chain hoặc parachain block mà không có bất kỳ nguy cơ nào về việc nó bị trả lại. Cách tốt nhất để đạt được điều đó
là có thỏa thuận Byzantine giữa những người xác nhận về trạng thái Polkadot và các parachains của nó.
Tuy nhiên, lược đồ tính khả dụng và hiệu lực 4.4.2 cũng có thể yêu cầu chúng tôi hoàn nguyên các khối, điều này
có nghĩa là nhận được thỏa thuận của Byzantine trên mọi khối, như trong Tendermint hoặc Algorand sẽ không phù hợp.
Tuy nhiên, điều này hiếm khi xảy ra vì rất nhiều stake-cổ phần sẽ bị chém khi chúng tôi làm điều này.
Do đó, chúng tôi muốn một lược đồ tạo ra các khối và thực thi chúng một cách lạc quan,
nhưng có thể mất một thời gian để hoàn thiện chúng. Do đó, cử tri GRANDPA cần phải chờ đợi sự đảm bảo
tính khả dụng và tính hợp lệ của một khối trước khi bỏ phiếu để hoàn thiện khối đó. Ngay cả tốc độ
chúng tôi hoàn thiện các khối có thể khác nhau - nếu chúng tôi không nhận được báo cáo về tính không hợp lệ và không có sẵn thì chúng tôi
có thể hoàn thành nhanh chóng, nhưng nếu chúng tôi làm như vậy thì chúng tôi có thể cần phải trì hoãn việc hoàn thiện trong khi chúng tôi thực hiện liên quan nhiều hơn

Do cách thức hoạt động giao thức thông điệp của Polkadot (XCMP 4.4.3), tốc độ truyền thông điệp
bị hạn chế bởi thời gian khối, nhưng không phải bởi thời gian thay đổi cuối cùng. Vì vậy, nếu chúng ta trì hoãn việc này nhưng cuối cùng không hoàn trả, thì sau đó tin nhắn đi qua vẫn nhanh chóng.

As a result of these requirements, we have chosen to separate the mechanisms for block production and finalising blocks as much as possible. In the next two sections, we describe the protocols
BABE and GRANDPA that do these respectively.

Do những yêu cầu này, chúng tôi đã chọn tách các cơ chế tiến triển khối và tạo khối càng nhiều càng tốt. Trong hai phần tiếp theo, chúng tôi mô tả các giao thức
BABE và GRANDPA tương ứng làm được những điều này.