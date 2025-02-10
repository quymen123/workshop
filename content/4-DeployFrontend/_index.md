---
title : "Deploy Frontend on AWS EC2"
date : "2025-02-08"
weight : 4
chapter : false
pre : " <b> 4. </b> "
---

**1. Deploy Frontend on AWS EC2**
- Clone code from github:
```bash
ssh -T git@github.com
git clone https://github.com/quymen123/ProjectAWS_FE.git
```
![ConnectPrivate](/workshop/images/4/1.png)

- Install library npm i:
```bash
ls
cd ProjectAWS_FE/
npm i
```
![ConnectPrivate](/workshop/images/4/2.png)

- Run build project:
```bash
npm run build
```
![ConnectPrivate](/workshop/images/4/3.png)

- Install pm2 so that when you exit the terminal, the app is still running:
```bash
npm install pm2 -g
```

- Run the app using pm2:
```bash
pm2 start npm --name nextjs-app -- run start -- -p 3333
```

- Run pm2 save to save the process:
```bash
pm2 save
```
![ConnectPrivate](/workshop/images/4/4.png)
