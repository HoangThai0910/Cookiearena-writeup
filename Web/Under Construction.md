# Under Construction #
## Description ##
Trang web không có gì ngoài 1 bức ảnh
## Solution ##
Mở thử ảnh trong tab mới thấy web lấy file working.png trong image.jsp. Mình đoán bài này có thể bị lỗi Path Traversal

![image](https://github.com/HoangThai0910/Cookiearena-writeup/assets/108949637/235d8870-ce5f-49b2-b0d1-94a17f974dff)

Trong tham số file mình thử nhập `../` nhiều lần để lùi về thư mục có file flag.txt. Sau khi nhập `../../../../../../flag.txt` thì có vẻ chúng ta đã tìm đúng vị trí file flag. Tuy nhiên web đang hiểu file text thành file ảnh nên không hiển thị được. Mình dùng lệnh wget để tải file về

![image](https://github.com/HoangThai0910/Cookiearena-writeup/assets/108949637/e4f2577c-87d1-4976-9552-1b544e7cdc4f)

Mở file lên và chúng ta có flag

Flag: CHH{unD3R_cOns7rUcTI0N_9fc464fc390361b5c17834d93d5bfa8d}
