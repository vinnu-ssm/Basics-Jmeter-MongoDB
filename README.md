** Basics MongoDB Testing using Jmeter**


##COMPONENTS

  - mongod - The database server.
  -  mongos - Sharding router.
  - mongo  - The database shell (uses interactive javascript).
  - Jmeter - To run test

##PRE-REQUISITE 
  - Download Jmeter http://mirrors.estointernet.in/apache//jmeter/binaries/apache-jmeter-5.2.1.zip
  - Put MongoDB Driver jar and groovy jar into jmeter lib/ext


  
##STEP TO RUN TEST 
  - Donwload mongoDB archive from https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.3.zip
  - Untar it and make database dir by command   mkdir -p ../data/db
  - Start MongoDB server by command  ./mongod --dbpath ../data/db/
  - Now run database shell by command ./mongo
  - Create database by command 'use jmeter_test'
  - Create Collection and Insert data into colleciton , follow below 
    db.createCollection("blazemeter_tutorial")
    db.blazemeter_tutorial.insert({"name": "john", "age" : 22, "location": "colombo"})
  - Now open JMX into Jmeter and run 
 
Note - Follow link for basic Mongo commands https://www.guru99.com/create-read-update-operations-mongodb.html


MONGO DB UTILITIES

  mongodump         - Create a binary dump of the contents of a database.
  mongorestore       - Restore data from the output created by mongodump.
  mongoexport        - Export the contents of a collection to JSON or CSV.
  mongoimport        - Import data from JSON, CSV or TSV.
  mongofiles            - Put, get and delete files from GridFS.
  mongostat            - Show the status of a running mongod/mongos.
  bsondump            - Convert BSON files into human-readable formats.
  mongoreplay        - Traffic capture and replay tool.
  mongotop            - Track time spent reading and writing data.
  install_compass    - Installs MongoDB Compass for your platform.

DRIVERS

  Client drivers for most programming languages are available at
  https://docs.mongodb.com/manual/applications/drivers/. Use the shell
  ("mongo") for administrative tasks.


DOCUMENTATION

  https://docs.mongodb.com/manual/

LEARN MONGODB

  https://university.mongodb.com/

