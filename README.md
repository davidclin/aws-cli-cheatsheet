# AWS CLI Cheatsheet

## How to get list of supported Availability Zones based on Instance Type
##### Change the instance type value so it matches yours. This example uses a g5.xlarge in us-east-1 region.
```
aws ec2 describe-instance-type-offerings --location-type availability-zone --filters Name=instance-type,Values=g5.xlarge --region us-east-1 --query 'InstanceTypeOfferings[].{InstanceType:InstanceType,
AvailabilityZone:Location}' --output table
```
![image](https://github.com/davidclin/aws-cli-cheatsheet/assets/6853545/da73c772-818b-45b7-8d4c-796a43994b49)

## How to quickly install AWS CLI on Windows
To update your current installation of AWS CLI on Windows, download a new installer each time you update to overwrite previous versions. AWS CLI is updated regularly. 
```
https://awscli.amazonaws.com/AWSCLIV2.msi
```

## How to quickly install AWS CLI on EC2 Ubuntu 18.04 Instance

```
# If using Ubuntu 10 or higher
# install aws cli via apt-get
sudo apt-get update
sudo apt-get install awscli
aws --version

# Install pip (not recommended for Ubuntu 10 or higher)
# https://askubuntu.com/questions/672808/sudo-apt-get-install-python-pip-is-failing
sudo apt-get install software-properties-common
sudo apt-add-repository universe
sudo apt-get update
sudo apt-get install python-pip




# Setup Credentials
aws configure
```
# If you're still having issues checkout
[( link )](https://stackoverflow.com/questions/36969391/how-to-upgrade-aws-cli-to-the-latest-version)
