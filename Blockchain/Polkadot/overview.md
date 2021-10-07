#　4.3　Consensus

Trong phần này, chúng tôi giải thích giao thức đồng thuận kết hợp của Polkadot bao gồm BABE: một
cơ chế tạo block của relay chain - cung cấp xác suất cuối cùng và GRANDPA
cung cấp tính cuối cùng có thể chứng minh, xác định được và hoạt động độc lập với BABE.
Không chính thức tính cuối cùng theo xác suất ngụ ý rằng sau khi thời gian nhất định trôi qua, một khối trong relay chain sẽ được hoàn thiện
với xác suất rất cao (gần bằng 1) và tính xác định cuối ngụ ý rằng một khối đã hoàn thành vẫn là khối cuối cùng
mãi mãi. Hơn nữa, tính chứng minh cuối cùng có nghĩa là chúng tôi có thể chứng minh cho các bên không tham gia tích cực vào
sự đồng thuận rằng một khối là cuối cùng.