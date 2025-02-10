---
title : "Triển khai Backend trên AWS EC2"
date : "2025-02-08"
weight : 3
chapter : false
pre : " <b> 3. </b> "
---

**1. Cài đặt Node.js và Git bằng nvm**
- Chuyển sang người dùng root:
```bash
sudo su -w
```
![ConnectPrivate](/workshop/images/3/1.png)
- Cài đặt nvm:
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
```
Nvm là trình quản lý phiên bản cho Node.js. Nó cho phép bạn cài đặt nhiều phiên bản Node.js và dễ dàng chuyển đổi giữa chúng.
![ConnectPrivate](/workshop/images/3/2.png)

- Kích hoạt nvm:
```bash
.  ~/.nvm/nvm.sh
```
Chúng ta cần kích hoạt nvm để có thể sử dụng trong phiên làm việc hiện tại.
![ConnectPrivate](/workshop/images/3/3.png)

- Sử dụng nvm để cài đặt Node.js:
```bash
nvm install node
```
Cài đặt phiên bản mới nhất của Node.js bằng nvm.
![ConnectPrivate](/workshop/images/3/4.png)

- Cài đặt git:
```bash
sudo apt-get update –y
sudo apt-get install git –y
```
Git cần thiết để clone kho lưu trữ mà chúng ta đã tạo trước đó.
![ConnectPrivate](/workshop/images/3/5.png)
![ConnectPrivate](/workshop/images/3/6.png)

**2. Kết nối SSH key GitHub với EC2**
- Tạo SSH key:
```bash
ssh-keygen -t ed25519 -C "your email"
```
Tạo dấu vân tay cho SSH key.
![ConnectPrivate](/workshop/images/3/7.png)

- Khởi động SSH-Agent:
```bash
eval "$(ssh-agent -s)"
```
Lệnh eval được sử dụng để khởi động SSH-Agent trong phiên làm việc hiện tại. SSH-Agent là một chương trình chạy nền giúp lưu trữ SSH key của bạn. Nó giúp xác thực với máy chủ từ xa mà không cần nhập mật khẩu mỗi lần.
![ConnectPrivate](/workshop/images/3/8.png)

- Thêm SSH key vào SSH-Agent:
```bash
ssh-add ~/.ssh/id_ed25519
```
![ConnectPrivate](/workshop/images/3/9.png)

- Sao chép SSH key và dán vào GitHub:
```bash
cat ~/.ssh/id_ed25519.pub
```
![ConnectPrivate](/workshop/images/3/10.png)
![ConnectPrivate](/workshop/images/3/11.png)

**3. Triển khai Backend trên AWS EC2**
- Clone mã nguồn từ GitHub:
```bash
ssh -T git@github.com
git clone https://github.com/quymen123/ProjectAWS_BE.git
```
![ConnectPrivate](/workshop/images/3/12.png)

- Cài đặt thư viện bằng npm:
```bash
cd ProjectAWS_BE/
npm i
```
![ConnectPrivate](/workshop/images/3/13.png)

- Cài đặt pm2 để ứng dụng vẫn chạy ngay cả khi thoát terminal:
```bash
npm install pm2 -g
```
![ConnectPrivate](/workshop/images/3/14.png)

- Chạy ứng dụng bằng pm2:
```bash
pm2 start src/index.js
```
![ConnectPrivate](/workshop/images/3/15.png)