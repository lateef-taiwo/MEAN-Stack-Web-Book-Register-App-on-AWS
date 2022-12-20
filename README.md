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
