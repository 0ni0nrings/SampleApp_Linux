# SampleApp_Linux
Sample Linux App for CodeDeploy Demo

# Link for Linux Sample App
[I'm an inline-style link](http://s3.amazonaws.com/aws-codedeploy-us-east-1/samples/latest/SampleApp_Linux.zip)

# User Data for Auto Scaling Group
#!/bin/bash
yum -y update
yum install -y ruby wget httpd
cd /home/ec2-user
curl -O https://aws-codedeploy-us-east-1.s3.amazonaws.com/latest/install
chmod +x ./install
./install auto
