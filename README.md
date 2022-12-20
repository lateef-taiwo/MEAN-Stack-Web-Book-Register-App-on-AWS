# MEAN-Stack-Web-Book-Register-App-on-AWS
This Repository explains the steps involved in creating and deploying a simple Web Book Register App on MEAN stack in AWS

![MEAN](./images/mean.jpeg)

## Step 1: Install NodeJs
Node.js is a JavaScript runtime built on Chrome’s V8 JavaScript engine. Node.js is used in this tutorial to set up the Express routes and AngularJS controllers.

* Update EC2 instance, that is Ubuntu

    `sudo apt update`

    ![update](./images/update.png)

* Upgrade ubuntu

    `sudo apt upgrade`

![upgrade](./images/upgrade.png)

* Add certificates
        
        sudo apt -y install curl dirmngr apt-transport-https lsb-release ca-certificates
 
        curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -

    ![certificate](./images/certificate.png)

    ![certificate](./images/Certificates.png)


* Install NodeJS
    `sudo apt install -y nodejs`

    ![node](./images/nodejs.png)

## Step 2: Install MongoDB
MongoDB stores data in adaptable documents that resemble JSON.
A database's fields can change from one document to another, and the data structure itself can change over time.

        sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 0C49F3730359A14518585931BC711F9BA15703C6
        
        echo "deb [ arch=amd64 ] https://repo.mongodb.org/apt/ubuntu trusty/mongodb-org/3.4 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.4.list

* Install MongoDB

    `sudo apt install -y mongodb`

    * If the above throws an error, try running 

            echo "deb [ arch=amd64 ] https://repo.mongodb.org/apt/ubuntu trusty/mongodb-org/3.4 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.4.list
    
    * then install gnupg

    `sudo apt-get install -y gnupg`

    ![gnupg](./images/gnupg.png)
    

    ![mongo](./images/mongo.png)
    ![mongo](./images/mongoo.png)

* Start The server

  `sudo service mongod start` 

* Verify that the service is up and running

    `sudo systemctl status mongod`
    ![mongo](./images/mongo%20start.png)