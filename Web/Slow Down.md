# Slow Down #
## Description ##
Challenge này vẫn là trang web cho phép đăng nhập bằng alice:alice hoặc bob:bob và vẫn có các chức năng chuyển tiền, mua flag
## Solution ##
Challenge này giống với `Be Positive` tuy nhiên đã bị filter số âm

Khi chuyển tiền thành công thì trả về khá lâu, dựa vào tên Challenge nữa thì mình đoán là bị lỗ hổng Race Condition. Mình sử dụng 2 trình duyệt để đăng nhập cùng 1 tài khoản sau đó chuyển tiền cho tài khoản còn lại. Phía chuyển chỉ tính 1 lần nhưng người nhận lại nhận được 2 lần

![image](https://user-images.githubusercontent.com/108949637/269591610-a089a0f4-5903-4e2d-865e-594dae3f2a75.png)

Đến đây thì mình mua flag thôi

Flag: CHH{ea5y_RaCe_CONd17iOn_34806440c8958c208985b933ca38ac7d}
