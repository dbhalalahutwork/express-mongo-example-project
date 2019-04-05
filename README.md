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
$ npm run migrate
```

### Run the Application

The project is preconfigured with a simple development web server. The simplest way to start this server is:

    npm start

### Run Test

```
npm test
```

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](#running-tests) for more information.

