# Youtube Downloader #
## Description ##
Đề cho chúng ta trang web có thể nhập link của video trên youtube, nhập xong sẽ hiện ra 1 câu lệnh gì đó và thumbnail của video đó
## Solution ##
Nhập thử `http://abc/;ls` thì thấy có thực thi lệnh nên bài này bị Command injection. Mình nhập `cat /flag.txt` để lấy flag nhưng bị thông báo url is not valid, thử bypass dấu cách thành `cat${IFS}/flag.txt` thì thành công lấy được flag

![image](https://user-images.githubusercontent.com/108949637/277730928-eda9abd5-47e2-409b-afa2-d627d3733b7e.png)

Flag: CHH{Ea5y_cOmmaND_inj3c7Ion_24d0201a7c3b77455d8d56b647373cfe}
