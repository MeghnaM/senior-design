# Server Access Overview

Our servers (Database and Web) are being hosted using Amazon Web Services Instances (one EC2, one RDS). The EC2 box is protected via a certificate, and the RDS one via username/pw logins.

## How to access the Web Server

The web server is an Ubuntu instance which you can remote into using the instructions below. Once we have an actual server program running on the box, you'll also be able to access the website off of the same URL.

1. download stockbox.pem from the google drive and store it in whatever directory you'll be remoting in from.
2. run this command: `chmod 400 stockbox.pem`
3. run this command `ssh -i stockbox.pem ubuntu@ec2-18-216-251-181.us-east-2.compute.amazonaws.com`

## How to access the Database Server

If you want to see how to access the database server through code, check `/home/bin/stockbox/stockboxpy/init_db.py` on the Web Server. Chances are that'll be handled by me (Chris) during the scaffolding phase though so it shouldn't be of much concern to anyone except maybe Meghna. The instructions below are for how to reach the database through an administrative tool so you can check out what's currently on the database and run queries against it. 

1. install pgAdmin (https://www.pgadmin.org/download/)
2. open pgAdmin and right click on "Servers," then choose "Create Server"
3. give it a name (probably just stockbox, doesn't matter), then go to the "Connection" tab and input:
hostname: `stockbox.c3zqtuvlnfqi.us-east-2.rds.amazonaws.com`
port: `5432`
username: `stockboxadmin`
password: `ehmsm2as`
4. voila, you should be good to go. If you have any questions lmk and I'll try to troubleshoot