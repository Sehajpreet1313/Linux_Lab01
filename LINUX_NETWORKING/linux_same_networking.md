# *🏠 Case 1: Mac and Ubuntu on the same network*
## *✅Step 1: Enable SSH on Ubuntu*

On Ubuntu, install and enable SSH:

sudo apt update
sudo apt install openssh-server
sudo systemctl enable ssh
sudo systemctl start ssh

![image](images/gui1.png)
Check it’s running:


sudo systemctl status ssh


##  ✅ Step 2: Find Ubuntu’s local IP address

Run:


hostname -I

![image](images/image1.png)
You’ll get something like 192.168.1.42.

## ✅ Step 3: Connect from Mac

On your Mac, open Terminal and run:


ssh username@192.168.1.42

Replace username with your Ubuntu username.

Enter your password when prompted — you’re in! ✅

![image](images/image2.png)
![image](images/image4.png)