Installing jenkins
setup the server
apt install openjdk-11-jre -y
go to jenkins.io - documentation - linux - choose os version and follow the steps





# jenkins


how to add jenkins slave

after setting up your jenkins master 
create another vm for jenkins

then go to jenkins master - manage plugins - manage nodes and clouds - new node - give it a name and create

description - adding apachevm as slave machine - execution.. how many job you want to exwecute simultenously - i choose 5

remote directory. - create a directory /root/slave1-jenkins
usage - use node as much as possible
launch method - launch agent via ssh
host verification stratey - non verify verification strategy
availablity - keep agent available as much as possible


now validate ..with a freestyle project
go to configure - build step - execute shell

you can also try with pipeline

you can also connect thru ssh priv key with another slave node



**************
nodejs on jenkins
go to manage jenkins - plugins - 


*******
execute shell scripts
cd /opt/springboot-maven-micro
sudo docker build -t junnlord/springboot-maven-micro:app .
sudo docker push junnlord/springboot-maven-micro:app
