# Hutwork UI

[![N|Solid](https://cdn.hutwork.com/wp-content/uploads/2018/03/logo-scroll-1.png)](https://www.hutwork.com/)

Hutwork gives teams just like yours collaboration and planning tools to create unique, highly targeted roadmaps. Check out the product roadmap software and see for yourself.

# Requirements

This project is an application skeleton for a typical [Node.js](https://nodejs.org/) web app.

  - Node 8
  - Git

## Getting Started
To get you started you can simply clone the repository:

```
git clone git@bitbucket.org:hutworkteam/hutwork-site.git
```
and navigate to the hutwork-site directory.
```
cd hutwork-site
```
and install the dependencies
```
npm install
```

### Run the Application

The project is preconfigured with a simple development web server. The simplest way to start this server is:

    npm run start
 
### Build the Application

The simplest way to build project is:

    npm run build
    
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
git clone git@bitbucket.org:hutworkteam/hutwork-site.git
```
and navigate to the hutwork-site directory.
```
cd hutwork-site
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

This will start UI node server at 3010 port so you have to redirect this port to 80,

You can do iptables port forwarding by adding following rules in iptables:
```
sudo iptables -t nat -I PREROUTING -p tcp --dport 80 -j REDIRECT --to-ports 3010
```
