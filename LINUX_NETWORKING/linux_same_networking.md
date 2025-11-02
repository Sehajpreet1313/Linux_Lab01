# *🏠 Case 1: Mac and Ubuntu on the same network*
## *✅Step 1: Enable SSH on Ubuntu*

On Ubuntu, install and enable SSH:

sudo apt update
sudo apt install openssh-server
sudo systemctl enable ssh
sudo systemctl start ssh

![image](<Screenshot 2025-10-29 213502.png>)
Check it’s running:


sudo systemctl status ssh


##  ✅ Step 2: Find Ubuntu’s local IP address

Run:


hostname -I

![image](<Screenshot 2025-10-29 214548-1.png>)
![image](<Screenshot 2025-10-29 214513-1.png>)
You’ll get something like 192.168.1.42.

## ✅ Step 3: Connect from Mac

On your Mac, open Terminal and run:


ssh username@192.168.1.42

Replace username with your Ubuntu username.

Enter your password when prompted — you’re in! ✅

![image](<WhatsApp Image 2025-10-30 at 09.07.56_e2c11759.jpg>)
![image](<WhatsApp Image 2025-10-30 at 09.05.28_a56ae977.jpg>)
![image](<WhatsApp Image 2025-10-30 at 09.05.29_33f98482.jpg>)
