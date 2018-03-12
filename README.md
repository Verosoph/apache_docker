# apache_docker

create a simple docker container with an apache Server

source: https://writing.pupius.co.uk/apache-and-php-on-docker-44faef716150

# how to use it:

clone the repo
go into the directory
build the docker container:                     $ docker build -t mysite .
run the docker without mounting a directory:   $ docker run -p 8080:80 -d mysite

call the site in the browser with localhost:8080

run the docker with mounting a directory:   $ docker run -p 8080:80 -d -v sourc_edirectory:/var/www/site mysite

source_directory is the directory where your project is located
