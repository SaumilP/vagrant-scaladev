# vagrant-scaladev
==========
vagrant for scala-dev environment with Ubuntu, Scala, Play Framework and MongoDB installed on it.

Requirements
===========
[vagrant](http://www.vagrantup.com/)

### Box includes ####

* [Ubuntu 12.04 (precise64)](http://releases.ubuntu.com/precise/)
* [Scala 2.10.3](http://www.scala-lang.org/)
* [Play Framework 2.2.1](http://www.playframework.com)
* [MongoDB 2.4.9](http://www.mongodb.org/)

Also installs:

* Git
* Vim
* Oracle Java 7
* Unzip
* wget

### Installation ###
* Clone scaladev to localhost ```git clone https://github.com/SaumilP/vagrant-scaladev.git```
* Fire command from terminal ```vagrant init```
* Start the Virtual Machine ```vagrant up```
* Once completed, connect using SSH ```vagrant ssh```
* Run ```postinstall.sh``` once connected to the VM
* Create new play app ```play new app```
* change directory ```cd app```
* start the play app ```play run```
* Visit started play app by going to browser: ```http://localhost:9000```

### Notes ###

Please not, current VM configuration is setup to use 1GB RAM, but if you require better performance increase upto 3024MB ( changes will be required in to ```vagrantfile```).

Once configuration changed, ```vagrant provision``` to update VM config changes and ```vagrant up``` startup the VM against new configuration.
