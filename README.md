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
