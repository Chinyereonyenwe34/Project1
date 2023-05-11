# Project1
## I started by connecting my instance to my terminal to access the ubuntu. 
![Instance connected to my terminal](https://github.com/Chinyereonyenwe34/Project1/assets/132712031/ff56963c-e92b-493f-a71b-6db2d114eb0a)
After that i proceeded to install my apache by running the command sudo apt install apache2. I followed by running the update and upgrade commands, which are sudo apt update and sudo apt upgrade respectively. 
I tested it to make sure the apache was running by running the command sudo systemctl status apache2. It showed me a green color and the caption "running"
### Installing mysql
Inorder to install mysql, i ran the command sudo apt install mysql-server 
![my-sql install](https://github.com/Chinyereonyenwe34/Project1/assets/132712031/6150b7e8-4c8d-4446-b0f3-49af69d45fc3)
After installing mysql, i tested it out to make sure it was running by running the command sudo systemctl status mysql.service and it showed running. images of mysql running can be found below
![mysql testing](https://github.com/Chinyereonyenwe34/Project1/assets/132712031/659714cb-cb58-4777-8105-e75fc5d79401)
#### Installing PHP
I installed php by running the command sudo apt install php
then i followed by running sudo apt install php libapache2-mod-php php-mysql 
![php install 2](https://github.com/Chinyereonyenwe34/Project1/assets/132712031/d86d9a04-1905-40d7-9fdd-3c781a81ff31)
I ran the command php -v to check the version of php installed as well.
##### Creating a virtual host with Apache
T create a virtual host, i used the github, i searched virtual host and went to the Aurthor Rover Wire/virtual host on github. I went to the global shortcut and followed the command there. I started by running
cd /usr/local/bin 
which took me to my local bin, then i ran this command
wget -O virtualhost https://raw.githubusercontent.com/RoverWire/virtualhost/master/virtualhost.sh  
which created the virtual host. I ran the ls command to ensure it was there. After which i applied permission to it by running 
sudo chmod +x virtualhost
I went back to my main directory by 
###### cd ~
then i ran the command 
###### sudo virtualhost create projectlamp
       images can be found below
 ![virtual host PROJECT LAMP](https://github.com/Chinyereonyenwe34/Project1/assets/132712031/60b76fdf-fa0f-493d-9d63-cf8ab8ba5c00)
    I enabled the virtual host with the command     sudo a2ensite projectlamp
I checked syntax errors and reloaded apache2.
Then i enabled php on the website. 





