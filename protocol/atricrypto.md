# Atricrypto
 
Bản nâng cấp của [[curve-stable-swap]], (may be asymetric tri-crypto), sử dụng cho nhiều token có giá khác nhau.

Công thức của curve stable swap như sau:

$$
S \times \sum_1^n x_i + \prod_1^n x_i = const
$$

Với x là "số lượng của token" trong pool. Tuy nhiên, nếu coi tất cả token đều có giá là 1, thì x có thể hiểu là giá trị của token trong pool:

$$
x_i = b_i \times p_i
$$

Trong đó: $b_i$ là balance của token i và $p_i$ là giá của nó. Như vậy hằng số của pool trở thành

Như vậy chỉ cần dự đoán được giá của token trong pool là có thể sử dụng được curve stable swap để có độ trượt giá tốt hơn uniswap.

Giá của token sẽ được tính toán lại mỗi khi có thay đổi trong pool, như đổi tiền, hoặc cung cấp hay rút bớt thanh khoản. Giá của 1 token sẽ được chọn là 1, các token còn lại được scale dựa trên giá của token dùng làm mốc đó.