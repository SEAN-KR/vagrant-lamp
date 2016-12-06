Vagrant LAMP
============

Want to test a new web app but don't want to affect your current Apache / MySQL / PHP system?
Applications like MAMP are great, but they don't make it easy to maintain multiple, separate
web roots.

If you find yourself needing quick to configure web stack, but also one that is customizable try this Vagrant project

Vagrant allows for Virtual Machines to be quickly setup, and easy to use.

And this project aims to make it very easy to spinup a complete LAMP stack in a matter of minutes.

Requirements
------------
* VirtualBox <http://www.virtualbox.org>
* Vagrant <http://www.vagrantup.com>
* Git <http://git-scm.com/> (Alternatively, SourceTree is a very good git client <https://www.sourcetreeapp.com/>.)

Usage
-----

### Startup
	$ git clone https://github.com/SEAN-KR/vagrant-lamp.git
	$ cd vagrant-lamp
	$ vagrant up

That is pretty simple.

### Connecting

#### Apache
The Apache server is available at <http://localhost:8088>

#### MySQL
Externally the MySQL server is available at port 3306, and when running on the VM it is available as a socket or at port 3306 as usual.
Username: root
Password: root

#### Phpmyadmin
You can access `phpmyadmin` at <http://localhost:8088/phpmyadmin>

#### Composer
Composer is a php dependency manager. It is installed globally, so you can use it in any of your projects by typing `composer`.

Technical Details
-----------------
* Ubuntu 14.04 64-bit
* Apache 2
* PHP 5.5
* MySQL 5.5
* Phpmyadmin
* Composer
* Bower

We are using the base Ubuntu 14.04 box from Vagrant. If you don't already have it downloaded
the Vagrantfile has been configured to do it for you. This only has to be done once
for each account on your host computer.

The web root is located in the project directory at `src` and you can install your files there.

And like any other vagrant file you have SSH access with

	$ vagrant ssh
