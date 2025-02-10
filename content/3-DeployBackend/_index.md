---
title : "Deploy Backend on AWS EC2"
date : "2025-02-08"
weight : 3
chapter : false
pre : " <b> 3. </b> "
---

**1. Install node and git using nvm**
- Change to root user:
```bash
sudo su -w
```
![ConnectPrivate](/workshop/images/3/1.png)
- Install nvm:
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
```
Nvm is a version manager for nodejs. It allows you to install multiple versions of nodejs and switch between them easily.
![ConnectPrivate](/workshop/images/3/2.png)

- Active nvm:
```bash
.  ~/.nvm/nvm.sh
```
We need to activate nvm so that we can use it in the current terminal session
![ConnectPrivate](/workshop/images/3/3.png)

- Use nvm to install node:
```bash
nvm install node
```
Install the latest version of node using nvm
![ConnectPrivate](/workshop/images/3/4.png)

- Install git:
```bash
sudo apt-get update –y
sudo apt-get install git –y
```
Git is need to clone the repo we created earlier
![ConnectPrivate](/workshop/images/3/5.png)
![ConnectPrivate](/workshop/images/3/6.png)

**2. Connect github ssh key to ec2 instance**
- Generate ssh key:
```bash
ssh-keygen -t ed25519 -C "your email"
```
Generate a fingerprint for the ssh key
![ConnectPrivate](/workshop/images/3/7.png)

- Eval the ssh-agent:
```bash
eval "$(ssh-agent -s)"
```
Eval is used to evaluate the ssh-agent in the current terminal session. The ssh-agent is a program that runs in the background and stores your ssh keys. The ssh-agent is used to authenticate you to the remote server without having to type your password every time.
![ConnectPrivate](/workshop/images/3/8.png)

- Add the ssh key to the ssh-agent:
```bash
ssh-add ~/.ssh/id_ed25519
```
![ConnectPrivate](/workshop/images/3/9.png)

- Copy ssh key and Paste into github:
```bash
cat ~/.ssh/id_ed25519.pub
```
![ConnectPrivate](/workshop/images/3/10.png)
![ConnectPrivate](/workshop/images/3/11.png)

**3. Deploy Backend on AWS EC2**
- Clone code from github:
```bash
ssh -T git@github.com
git clone https://github.com/quymen123/ProjectAWS_BE.git
```
![ConnectPrivate](/workshop/images/3/12.png)

- Install library npm i:
```bash
cd ProjectAWS_BE/
npm i
```
![ConnectPrivate](/workshop/images/3/13.png)

- Install pm2 so that when you exit the terminal, the app is still running:
```bash
npm install pm2 -g
```
![ConnectPrivate](/workshop/images/3/14.png)

- Run the app using pm2:
```bash
pm2 start src/index.js
```
![ConnectPrivate](/workshop/images/3/15.png)