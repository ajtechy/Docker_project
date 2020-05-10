# Docker_project
REQUIREMENTS:

1. docker installed in your system

2. owncloud:latest  and mysql:5.7 image (cointainer image)

3. docker-compose

# Introduction 
Docker project on launching owncloud in my system by using docker container over rhel 8 and u can put your gb's of data here which will be safe and secure for us.


# Steps

step 1 : git clone https://github.com/ajtechy/Docker_project.git

step 2 : download images if not available using following command
1.  docker pull owncloud:latest
2.  docker pull mysql:5.7

step 3 : download mysql client if not download using following command
1.  yum install mysql

step 4 : inside any dir create ur docker-compose.yml and paste the code of my docker-compose.yml Then run the following command on cmd
1.  docker-compose up -d
  
step 5 : get container id of both images using following command
1.  docker ps 

step 6 : get IP of your owncloud images using following command
1.  docker inspect < id of owncloud container > | grep IP
  
Step 6 : put this IP in firefox and their will be owncloud home page in front of you where u can upload your data and enjoy. 
1.  <IP>/index.php
  
for example  172.18.0.2/index.php

