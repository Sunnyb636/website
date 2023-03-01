# website
 
 Dockerfile :
 FROM ubuntu
RUN apt-get update
RUN apt install apache2 -y
RUN rm /var/www/html/index.html
ADD .  /var/www/html/
CMD apachectl -D FOREGROUND


master.sh script file:

sudo apt install docker.io -y

sudo apt install openjdk-11-jdk -y

wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -

sudo sh -c 'echo deb https://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'

sudo apt-get update

sudo apt-get install jenkins -y




slave.sh script file:

sudo apt install docker.io -y

sudo apt install openjdk-11-jdk -y


