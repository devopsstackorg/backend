$git clone https://github.com/devopsstackorg/backend.git

$cd backend

$docker image build -t <image_name> .

$docker run -d --name <container_name> -e MYSQL_ROOT_PASSWORD=Root_123 <image_name>

Step 3: create database and user for MySQL and import data into database $docker exec -it <container_name> sh

$mysql -u root -p

mysql>create database indigo;

mysql>CREATE USER '<user_name>'@'%' IDENTIFIED BY '';

mysql>GRANT ALL ON . TO ''@'%';

mysql>FLUSH PRIVILEGES;

$git clone https://github.com/krishnamaram2/WebApp.git

$cd WebApp/binary $mysql -u <user_name> -p indigo < indigo.sql
