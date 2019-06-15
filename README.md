# rocketchat
-install docker-compose
-clone the project 
-cd to Project 
#sudo mkdir -p data/runtime/db
#sudo mkdir -p data/dump
-set this record in your hostfile : 127.0.0.1    chat.inumio.com          chat
#docker-compose up --scale rocketchat=2 
-the service is available on :
http://chat.inumio.com/
-you can check which conatiner is runnig with : #docker ps
 docker ps
CONTAINER ID        IMAGE                 COMMAND                  CREATED             STATUS                                             NAMES
ac24811e70d1        dockercloud/haproxy   "/sbin/tini -- docke…"   42 minutes ago      Up 4 seconds      
d4de85734abf        rocket.chat:latest    "bash -c 'for i in `…"   42 minutes ago      Up 6 seconds                                     chat_rocketchat_2
583551f37b75        rocket.chat:latest    "bash -c 'for i in `…"   42 minutes ago      Up 7 seconds                                     chat_rocketchat_1
5c0c3df07a37        mongo                 "docker-entrypoint.s…"   2 hours ago         Up 9 seconds                                 chat_mongo_1

