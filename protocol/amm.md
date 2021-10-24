# AMM

Auto market maker #amm. Hiểu đơn giản là một giao thức trao đổi token tự động. Khác với các sàn giao dịch tập trung nơi người mua và người bán trao đổi tiền với nhau, mỗi khi có ai đó muốn bán thì phải có một người nào đó muốn mua giao dịch mới được thực hiện,. AMM cho phép giao dịch diễn ra ngay tức thì. Thông thường sẽ thực hiện thông qua một #liquidity_pool, là nơi những người có thanh khoản nhàn rỗi đóng góp vào. Những người này sẽ thu được lợi tức từ phí giao dịch của protocol

## Liquidity pool

Để giao dịch được tự động diễn ra, cần có liquidity pool. Hiểu đơn giản là một smart contract (C) chứa một số lượng các token sẽ được trao đổi. Giả sử một pool chứa n token T1... Tn, với số lượng A1.. An. Một giao dịch trao đổi diễn ra bằng cách chuyển x đồng Ti vào pool và smart contract (C) sẽ chuyển lại cho người dùng đó một số lượng y đồng Tj, với y được thuật toán AMM quyết định. Thuật toán AMM tương đối phong phú và ngày càng được hoàn thiện. 

Lượng token trong pool được gọi là thanh khoản #liquidity và do người dùng tự nguyện đóng góp để nhận về lợi nhuận từ phí giao dịch.