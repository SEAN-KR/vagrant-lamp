# 프로젝트팀 을 위한 #Slack  
Androidthings Slack 팀 그룹이 있습니다  
참여하시고 싶으신 분은  
https://androidthingskorea.herokuapp.com/  
이메일주소를 입력하시면 초대장 발송됩니다  

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


## 빌드된 이미지

https://drive.google.com/drive/folders/0B-y5Szi9BBVFS0NHS29TQ2d1elk?usp=sharing
