# OpenVAS-TEST
openvas demo

Installation

Phần tải này sẽ cài đặt OpenVAS trên máy Ubuntu cảu tôi. Việc cài đặt OpenVAS có thể rất phức tạp vì nó có nhiều phần phụ thuộc. 

Ở đây tôi sẽ cài docker, docker là một nền tảng cho developers và sysadmin để develop, deploy và run application với container. Nó cho phép tạo các môi trường độc lập và tách biệt để khởi chạy và phát triển ứng dụng và môi trường này được gọi là container.

Khi cần deploy lên bất kỳ server nào chỉ cần run container của Docker thì application của bạn sẽ được khởi chạy ngay lập tức.

![image](https://github.com/user-attachments/assets/2b04bc7e-1fe3-4237-93a9-aa439be8974d)

Tiếp đến, tôi sẽ khởi tạo một vùng chứa OpenVAS với tất cả các phụ thuộc đã được cài đặt bằng câu lệnh sau : 

**sudo docker run -d -p 8443:443 --name openvas mikesplain/openvas**

![image](https://github.com/user-attachments/assets/876ecb0f-b212-4199-9637-fed9696438cb)

Sau khi thiết lập vùng chứa thành công, chúng ta sẽ có thể truy cập OpenVAS theo dạng web.

truy cập vào bất cứ trình duyệt(browser) nào, để truy cập **https://127.0.0.1:8443**

![image](https://github.com/user-attachments/assets/2414c021-2c62-468a-b473-324ecf294bd0)


và đây là giao diện của OpenVAS:

![image](https://github.com/user-attachments/assets/f7c565bb-2229-4f7a-8735-b611bcdff61d)

OpenVASE có khá nhiều chức năng, ở đây mình sẽ thử sử dụng SCAN, bằng cách nhấn vô mục menu -> scan -> task.

![image](https://github.com/user-attachments/assets/05687c83-2e58-40de-a520-61cea1532e73)

Đây là giao diện cài đặt của scan:

![image](https://github.com/user-attachments/assets/53b059e7-5e55-4d2a-bf99-e9884f51d964)

Sau khi thành lập 1 task, thì mình sẽ scan thử: 

![image](https://github.com/user-attachments/assets/4f7c83a2-e317-4adf-a79b-4b63be83608f)

Ở đây, sau khi scan xong nó lại hiện dead, nên mình thử lại ip khác:
![image](https://github.com/user-attachments/assets/196a838f-b0d5-4ce2-83df-fd81356c4e77)

![image](https://github.com/user-attachments/assets/0cb29ddb-c2f7-4bfc-963c-b0653981ee48)

Và OpenVAS đã cho mình kết quả

![image](https://github.com/user-attachments/assets/e0e7cb0b-d803-4e41-8eb8-5758a1a9a8d9)

