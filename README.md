# SampleApp_Linux
Sample Linux App for CodeDeploy Demo. This is the original app from AWS. The ZIP file attached to this repo is modified version.

# Link for Linux Sample App
[Original Linux Sample App Link](http://s3.amazonaws.com/aws-codedeploy-us-east-1/samples/latest/SampleApp_Linux.zip)

# User Data for Auto Scaling Group
```
#!/bin/bash
yum -y update
yum install -y ruby wget httpd
cd /home/ec2-user
curl -O https://aws-codedeploy-us-east-1.s3.amazonaws.com/latest/install
chmod +x ./install
./install auto
```
