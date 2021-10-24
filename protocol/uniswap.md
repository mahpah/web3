# Uniswap

Thuật toán #uniswap khá đơn giản, sử dụng cho pool chỉ gồm 2 token. Lượng token trong pool được giữ sao cho tích của chúng là hằng số khi trao đổi (constant product)

Ví dụ, tại thời điểm trước khi trao đổi trong pool có chứa x đồng A và y đồng B, đặt k là tích của chúng:

$$
a \times b = k
$$


Ngưởi dùng muốn trao đổi x đồng A và nhận lại y đồng B thì x và y cần thoả mãn:

$$
(a + x) \times (b - y) = k
$$

Suy ra y tính bằng công thức

$$
y = b - \frac{a \times b}{a + x}
$$
