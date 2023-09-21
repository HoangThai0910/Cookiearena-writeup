# Be Positive
## Description ##
Đề cho chúng ta một trang web đăng nhập. Sau khi đăng nhập bằng alice:alice hoặc bob:bob giao diện trang web hiện ra như sau
![image](https://user-images.githubusercontent.com/108949637/269579323-0f742ea2-e2a5-4545-879f-e1701b55aedd.png)
## Solution ##
Trong mục Market chúng ta có thể mua flag với `3001$` nhưng số dư trong tài khoản chỉ có `1500$`. Mình thử vào phần Transfer thì thấy web cho phép chúng ta nhập vào số tiền rồi chuyển cho alice/bob
![image](https://user-images.githubusercontent.com/108949637/269582434-8a23e65b-c395-4f99-8637-074a4ad8327e.png)

Sau khi chuyển tiền thì hệ thống sẽ trừ tiền của chúng ta. Vậy nếu chúng ta nhập vào 1 số âm thì khi trừ đi số âm chẳng phải sẽ thành cộng cho tài khoản chúng ta sao. Mình mở burpsuite và sửa `amount` thành số âm
![image](https://user-images.githubusercontent.com/108949637/269583449-2a03d34f-f58b-4d13-a524-bff789ecfcbc.png)

Sau khi chuyển đi thì tài khoản của chúng ta thực sự đã được cộng thêm
![image](https://user-images.githubusercontent.com/108949637/269584825-89c1bf72-5922-4caa-a28b-f0e7cace8e12.png)

Đến đây thì ta tiến hành mua flag thôi. Lần đầu mua sẽ ra fake flag, tiếp tục mua lần nữa là ra real flag

Flag: CHH{BE_cAr3fUL_WitH_NE6ATIV3_NumBeR_c39fd11c08510b52273e732a2995048d}
