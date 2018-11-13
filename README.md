# How to quicly install AWS CLI on EC2 Ubuntu 18.04 Instance

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
