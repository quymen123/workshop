---
title : "Kiểm tra và đánh giá ứng dụng"
date :  "2025-02-08" 
weight : 5 
chapter : false
pre : " <b> 5. </b> "
---

**1. Sao chép Địa chỉ IPv4 công khai và dán vào trình duyệt:**
```bash
http://54.89.223.174:8888/
```
- Cổng (Port): 8888 là số cổng. Cổng được sử dụng để xác định một dịch vụ trên máy chủ. Trong trường hợp này, cổng 8888 thường được dùng cho các ứng dụng web, proxy hoặc các dịch vụ khác.
![ConnectPrivate](/workshop/images/5/1.png)

**2. Giao diện trang đăng ký**
![ConnectPrivate](/workshop/images/5/2.png)

- Trang đăng ký có kiểm tra định dạng email và không cho phép bỏ trống các trường.
![ConnectPrivate](/workshop/images/5/3.png)

- Sau khi đăng ký thành công, thông tin sẽ được gửi đến MongoDB và có thể tiến hành đăng nhập.
![ConnectPrivate](/workshop/images/5/4.png)

**3. Giao diện trang đăng nhập**
![ConnectPrivate](/workshop/images/5/5.png)
- Nhập email và mật khẩu đã đăng ký để đăng nhập.
![ConnectPrivate](/workshop/images/5/6.png)
- Đăng nhập thành công, nhấn thoát để đăng xuất.