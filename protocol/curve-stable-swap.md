# Curve stable swap

Curve là một [[AMM]] dùng cho stable coin, hoặc rộng hơn là cho các đồng có giá bằng nhau.
Curve kết hợp thuật toán của [[Uniswap]] cùng với thuật toán dạng constant-sum

Thuật toán của uniswap là constant product, tức lượng token trong pool luôn thỏa mãn 

$$
\prod_1^n {x_i} = const
$$

Trái lại thuật toán constant sum lại yêu cầu tổng số lượng các token là hằng số

$$
\sum_1^n x_i = const
$$

Curve kết hợp 2 công thức này, bằng cách tìm ra một hệ số $S$ để

$$
S \times \sum_1^n x_i + \prod_1^n x_i = const
$$

Với giả thiết các token có giá bằng nhau, ta có thể đặt $\sum_1^n x_i = D$, và tính tích của chúng bằng $\prod_1^n x_i = (\frac {D} {n})^{n}$.

Khi đó hằng số ở trên sẽ là

$$
S \times D + (\frac {D} {n})^{n} = const
$$

Chọn $S = \chi D^{n-1}$, hằng số trên viết thành

$$
\chi D^{n} + (\frac {D} {n})^{n} = const
$$

Sau một số tính toán phức tạp chọn được

$$
\chi = \frac{A \prod x_i}{(D/n)^n}
$$

Thay vào hệ thức và biến đổi để triệt tiêu biến số, nhận được 

$$
An^n \sum{x_i} + D = ADn^n + \frac{Dn^{n+1}}{n^n\prod{x_i}}
$$