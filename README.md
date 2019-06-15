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

I realized that for scaling services in docker It's pretty bettrer to use docker swarm , but I have'nt time to try it . I almost interested in it , of course kubernetes technology manage it in the best way . but I hope can make some time to try it out .
