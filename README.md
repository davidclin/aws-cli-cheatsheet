# How to quicly install AWS CLI on EC2 Ubuntu 18.04 Instance

```
# Install pip  
# https://askubuntu.com/questions/672808/sudo-apt-get-install-python-pip-is-failing
sudo apt-get install software-properties-common
sudo apt-add-repository universe
sudo apt-get update
sudo apt-get install python-pip


# Install
sudo apt-get update
sudo apt-get install python-pip
pip install awscli --upgrade --user
sudo apt-get update
sudo apt-get install awscli
pip install awscli --upgrade --user
aws --version

# Setup Credentials
aws configure
```
# If you're still having issues checkout
[( link )](https://stackoverflow.com/questions/36969391/how-to-upgrade-aws-cli-to-the-latest-version)
