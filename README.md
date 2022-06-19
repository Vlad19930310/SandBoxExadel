#Task 2 Working with AWS Cloud, install Apache web server
Create 2 instance: Linux Amazon, Linux Ubuntu with Key pair in AWS cloud
Create VPC 
Create subnet
Create security group
Configure Route Table (Destination 0.0.0.0/0, Target<your Internet Gateway>)
Create, Attach Internet Gateway
Configure Inbound rules: SSH:22, HTTP:80, ICMP IPv4
Connect to Instances from client "MobaExterm"
Check ping from host to instances, from instance to instance
Configure,connect SSH from instance to instance with key pair
Install Apache to Amazon Linux "sudo yum install httpd; sudo service httpd start; sudo service httpd status; chkconfig on (Apache will autostart after rebooting OS)
Create html web page "var/www/html/index.html" 
Check web page from host
Check web page from Ubuntu instance (sudo apt-get install curl wget lynx w3m elinks - utilti to display web page)
Put web page content to variable (page="$(curl http://34.228.59.210/))" 
Print web page content in terminal echo $page
The result is http://34.228.59.210/
