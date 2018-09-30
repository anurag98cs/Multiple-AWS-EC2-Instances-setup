# Multiple-AWS-EC2-Instances-setup


-----------------AWS EC2 instance #1-----------------------------------------------------------------
Jenkins Installation:


sudo apt-get update
sudo apt-get install apache2
wget -q -O - https://pkg.jenkins.io/debian/jenkins-ci.org.key | sudo apt-key add -
sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
sudo apt-get update
sudo apt-get install jenkins


-----------------AWS EC2 instance #2-----------------------------------------------------------------

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
sudo apt-get update
apt-cache policy docker-ce
sudo apt-get install -y docker-ce




sudo apt-get install chromium-browser
sudo apt-get install chromium-chromedriver
sudo apt-get install default-jdk


sudo docker run -it -d ubuntu

----Installing ubuntu in Docker image
sudo docker run -it -d ubuntu
sudo docker run -it -d -p 80:80 <Image ID>
sudo docker exec -it <Docker Container ID> bash
Now you are in Docker's Ubuntu bash prompt
apt-get update
apt-get install apache2
service apache2 restart
