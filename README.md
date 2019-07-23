### devbox에서 docker-maven-plugin 으로 이미지 빌드하기 ###
> docker run -itd --name devbox -v /var/run/docker.sock:/var/run/docker.sock -v /usr/local/bin/docker:/usr/bin/docker moricom/devbox
> docker exec -it devbox bash  
>> git clone https://github.com/moricom2/egovframe-sample.git  
>> cd egovframe-sample  
>> git checkout devbox  
>> mvn clean package docker:build  
>> exit
