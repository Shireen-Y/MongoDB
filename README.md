1. Make new repo named MongoDB
2. ``cd`` into ``tests``
3. ``rake spec``
4. Should get 4 failures
5. ``cd..`` then ``cd MongoDB/``
6. ``vagrant up``
7. ``vagrant ssh``

## Installing MongoDB
1. Copy and paste this:
    ``wget -qO - https://www.mongodb.org/static/pgp/server-3.2.asc | sudo apt-key add -``
      - It should respond with 'OK'

## Create a list for MongoDB
1. Run this :
      ``echo "deb http://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/3.2 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.2.list``
2. Reload the local package database:
      ``sudo apt-get update``

## Installing MongoDB packages
1. Install the latest stable version:
      ``sudo apt-get install -y mongodb-org=3.2.20 mongodb-org-server=3.2.20 mongodb-org-shell=3.2.20 mongodb-org-mongos=3.2.20 mongodb-org-tools=3.2.20``

## Start Mongodb
      ``sudo service mongod start``

## Verify that is has started successfully
        ``sudo service mongod status``

## To Stop MongoDB
        ``sudo service mongod stop``

## To Restart it
        ``sudo service mongod restart``

## Begin using MongoDB
        ``mongo``
