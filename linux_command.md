Clear Screen
=============
clear


Get linux version
=======================
1. lsb_release -a
1. cat /etc/os-release


PHP Version upgrade My case is php 5.4 to php 5.7
=================================================
01. Remove Older PHP
================
sudo yum remove php-cli mod_php php-common

02. install epel release
sudo yum install epel-release yum-utils -y;

03. Download and Install remirepo using yum command
sudo yum install http://rpms.remirepo.net/enterprise/remi-release-7.rpm

04. To configure PHP 7.0 repository
sudo yum-config-manager --enable remi-php70

05. Install PHP
sudo yum install php php-common php-opcache php-mcrypt php-cli php-gd php-curl php-mysql -y



HTTP server restart
===================================
sudo service httpd restart


Update Yam
======================
sudo yum update