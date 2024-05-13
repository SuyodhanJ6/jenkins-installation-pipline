# jenkins-installation-pipline

## Perform these commands on the EC2 instance

### YUM 
sudo yum update
sudo yum install docker
sudo usermod -a -G docker ec2-user
id ec2-user
newgrp docker
sudo systemctl enable docker.service
sudo systemctl start docker.service
sudo systemctl status docker.service
sudo yum install git
which git ---> set git path in Jenkins
chmod 777 /var/run/docker.sock

## UBUNTU
sudo apt update
sudo apt install docker.io
sudo usermod -aG docker $USER
id $USER
newgrp docker
sudo systemctl enable docker.service
sudo systemctl start docker.service
sudo systemctl status docker.service
sudo apt install git
which git # Sets git path in Jenkins
sudo chmod 777 /var/run/docker.sock


## Working
sudo apt update
sudo apt install docker.io
sudo usermod -aG docker jenkins
sudo systemctl enable jenkins
sudo systemctl start jenkins
sudo systemctl status jenkins

## Plugins to install in Jenkins
Pipeline: AWS Steps
CloudBees AWS Credentials Plugin
All Git plugin
Amazon ECR Pipeline
Docker API Plugin
Docker Commons Plugin
Docker Pipeline
Docker plugin
Docker workflow
GitHub Integration Plugin Version0.5.0 GitHub Integration Plugin for Jenkins

GitHub plugin Version1.37.0 This plugin integrates GitHub to Jenkins. Report an issue with this plugin

Pipeline: GitHub Version2.8-138.d766e30bb08b
