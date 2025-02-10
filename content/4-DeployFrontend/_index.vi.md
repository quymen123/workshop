---
title : "Triển khai Frontend trên AWS EC2"
date : "2025-02-08"
weight : 4
chapter : false
pre : " <b> 4. </b> "
---

**1. Triển khai Frontend trên AWS EC2**
- Clone mã nguồn từ GitHub:
```bash
ssh -T git@github.com
git clone https://github.com/quymen123/ProjectAWS_FE.git
```
![ConnectPrivate](/workshop/images/4/1.png)

- Cài đặt thư viện bằng npm:
```bash
ls
cd ProjectAWS_FE/
npm i
```
![ConnectPrivate](/workshop/images/4/2.png)

- Chạy lệnh build dự án:
```bash
npm run build
```
![ConnectPrivate](/workshop/images/4/3.png)

- Cài đặt pm2 để ứng dụng vẫn chạy ngay cả khi thoát terminal:
```bash
npm install pm2 -g
```

- Chạy ứng dụng bằng pm2:
```bash
pm2 start npm --name nextjs-app -- run start -- -p 3333
```

- Lưu tiến trình pm2 để tự động khởi động lại khi hệ thống khởi động lại:
```bash
pm2 save
```
![ConnectPrivate](/workshop/images/4/4.png)
