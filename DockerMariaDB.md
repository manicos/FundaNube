# Show Docker containers
docker ps

#Show Docker images
docker images

#Download MariaDB Image
docker pull mariadb

#Clean system
Docker system prune

#DELETE CONTAINER
docker container rm containername

#Mount Maria DB
docker run -d --name myfirstdb -p 34672:3306 -v /Users/alfredobolio/Docker/dbconfig/:/etc/mysql/conf.d -v /Users/alfredobolio/Docker/dbfiles/:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=1234 -e MYSQL_DATABASE=mytfirstdb mariadb

#Shell for the docker container
docker exec -it containername bash

#Stop container
docker stop containername

#Start container
docker start containername

#Restart container
docker restart containername
