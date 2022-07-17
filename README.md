## LAMP stack built with Docker Compose

A basic LAMP stack environment built using Docker Compose. It consists of the following:

- PHP
- Apache
- MySQL
- phpMyAdmin
- Redis

Use appropriate php version as needed:

- 7.4.3

## Installation

- Clone this repository on your local computer
- configure .env as needed
- Run the `docker-compose up -d`.

```shell
git clone https://github.com/sprintcube/docker-compose-lamp.git
cd docker-compose-lamp/
cp sample.env .env
// modify sample.env as needed
```

Starting the LAMP Server:
```
sudo docker-compose up -d

```

To show the list of running container:
```
docker-compose ps
```

Running an Interactive Shell in a Docker Container:
```
docker exec -it container-name sh
```

Exit for a Running Container:
```
# exit
```

Find the IP address of a Running Container:
```
# hostname -i
```

Your LAMP stack is now ready!! 
You can access Web Server via: `http://localhost:8080`
You can access PhpMyAdmin via: `http://localhost:5000`

Stop Running Container:
```
docker-compose down or stop

```

Find the actual name of the volume with the following command:
```
docker volume ls

```

Find the actual name of the volume with the following command:
```
docker volume rm VOLUME_NAME

```

Remove one or more specific containers:
```
docker rm ID_or_Name ID_or_Name

```