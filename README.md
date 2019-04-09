# Hutwork API

[![N|Solid](https://cdn.hutwork.com/wp-content/uploads/2018/03/logo-scroll-1.png)](https://www.hutwork.com/)

Hutwork gives teams just like yours collaboration and planning tools to create unique, highly targeted roadmaps. Check out the product roadmap software and see for yourself.

# Requirements

This project is an application skeleton for a typical [Node.js](https://nodejs.org/) web app.

  - Node 8
  - Git
  - MongoDB

## Getting Started
To get you started you can simply clone the repository:

```
git clone git@bitbucket.org:hutworkteam/hutwork_api.git
```
and navigate to the hutwork_api directory.
```
cd hutwork_api

```
and install the dependencies
```
npm install
```

### MongoDB
The project uses MongoDB as a database. If you are on Mac and using Homebrew package manager the installation is as simple as `brew install mongodb`.
If you on linux please check this link to install mongoDB 
https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/

### Start the MongoDB server
First we need to create the `db` directory where the database files will live in. In your terminal navigate to the `root` of your system by doing `cd ..` until you reach the top directory. You can create the directory by running `sudo mkdir -p /data/db`. Now open a different tab in your terminal and run `mongod` to start the Mongo server.

## Run mongo migrate

```
$ npm run migrate up
```

### Run the Application

The project is preconfigured with a simple development web server. The simplest way to start this server is:

    npm run start

### Run Test

```
npm run test
```

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](#running-tests) for more information.

### Run Application on AWS server 

Connect AWS console with this command in ubuntu and mac (you must have pem file with same directory) for window use putty with ppk
```
ssh -i HW-KP-01.pem ubuntu@18.216.71.35

```
Now you have to navigate [/var/www/html](#/var/www/html) directory
```
cd /var/www/html
```
Next follow same step from [Getting Started](#Getting Started) section to setup API from git

also [Requirements](#Requirements) section is same for server also

### Run Application on AWS server 

Connect AWS console with this command in ubuntu and mac (you must have pem file with same directory) for window use putty with ppk
also pem file must have valid permissions for execute 
```
chmod 400 HW-KP-01.pem
```
```
ssh -i HW-KP-01.pem ubuntu@18.216.71.35
```

also [Requirements](#Requirements) section is same for server also
need to install git and node 8
```
apt-get update
apt-get install git-core
```

```
sudo apt-get install curl python-software-properties
curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
apt-get install nodejs
```

Now you have to navigate [/var/www/html](#/var/www/html) directory
```
cd /var/www/html
```

Next follow same step from [Getting Started](#Getting Started) section to setup API from git

To get you started you can simply clone the repository:
```
git clone git@bitbucket.org:hutworkteam/hutwork_api.git
```
and navigate to the hutwork_api directory.
```
cd hutwork_api
```
and install the dependencies
```
npm install
```
[Note](#Note) Some case `npm install`  will not work that case you have to use `yarn install` in this case you need to install `yarn`  
```
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt update
sudo apt install yarn
```
### MongoDB
The project uses MongoDB as a database. please check this link to install mongoDB 
https://docs.mongodb.com/manual/tutorial/install-mongodb-on-ubuntu/

### Start the MongoDB server
First we need to create the `db` directory where the database files will live in. In your terminal navigate to the `root` of your system by doing `cd ..` until you reach the top directory. You can create the directory by running `sudo mkdir -p /data/db`. Now open a different tab in your terminal and run `mongod` to start the Mongo server.

## Run mongo migrate

```
$ npm run migrate up
```

### Run the Application

The project is preconfigured with a simple development web server. The simplest way to start this server is:

    npm run start
    
This will run on 3000 port
