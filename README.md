# Mongodb
Mongodb projects
## Installation (Linux)

sudo vim /etc/yum.repos.d/mongodb.repo 

Add the below content::

[Mongodb]
name=MongoDB Repository
baseurl=https://repo.mongodb.org/yum/redhat/8/mongodb-org/4.4/x86_64/
gpgcheck=1
enabled=1
gpgkey=https://www.mongodb.org/static/pgp/server-4.4.asc

## Starting server
sudo dnf install mongodb-org mongodb-org-server 

sudo systemctl enable mongod.service 
sudo systemctl start mongod.service 

mongod --version 
