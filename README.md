Installation and deploing:

Dependencies:
java
ant
ivy
jetty

Building, and deploing example for ubuntu:

sudo apt-get install ant
sudo apt-get install ivy
sudo apt-get install jetty

sudo cp /usr/share/java/ivy.jar /usr/share/ant/lib/ivy.jar

git clone https://github.com/alexglue/unicorn.git
cd ./unicorn
ant retrieve default_conf war
sudo mv ./dist/unicorn.war /usr/share/jetty/webapps/
sudo service jetty restart

Now your service will be available from http://localhost:8080/unicorn/
