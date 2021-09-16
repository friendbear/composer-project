# PHP Ubuntu21.0.4 on RaspberryPi4b

## composer demo

* see [install_php_composer_ubuntu](https://linuxhint.com/install_php_composer_ubuntu)


```sh
curl -sS https://getcomposer.org/installer | php
sudo mv composer.phar /usr/local/bin/composer
sudo chmod +x /usr/local/bin/composer
source .bashrc
mkdir composer-project
cd composer-project/
composer require cakephp/chronos
```

run

```sh
$ php demo.php
```


### geoip.php

```sh
$ sudo apt install php-curl
[sudo] password for pi: 
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  php7.4-curl
The following NEW packages will be installed:
  php-curl php7.4-curl
0 upgraded, 2 newly installed, 0 to remove and 0 not upgraded.
Need to get 31.2 kB of archives.
After this operation, 144 kB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 http://ports.ubuntu.com/ubuntu-ports hirsute-updates/main arm64 php7.4-curl arm64 7.4.16-1ubuntu2.1 [29.2 kB]
Get:2 http://ports.ubuntu.com/ubuntu-ports hirsute/main arm64 php-curl all 2:7.4+76ubuntu1 [2,008 B]
Fetched 31.2 kB in 1s (23.3 kB/s)    
Selecting previously unselected package php7.4-curl.
(Reading database ... 222455 files and directories currently installed.)
Preparing to unpack .../php7.4-curl_7.4.16-1ubuntu2.1_arm64.deb ...
Unpacking php7.4-curl (7.4.16-1ubuntu2.1) ...
Selecting previously unselected package php-curl.
Preparing to unpack .../php-curl_2%3a7.4+76ubuntu1_all.deb ...
Unpacking php-curl (2:7.4+76ubuntu1) ...
Setting up php7.4-curl (7.4.16-1ubuntu2.1) ...

Creating config file /etc/php/7.4/mods-available/curl.ini with new version
Setting up php-curl (2:7.4+76ubuntu1) ...
Processing triggers for libapache2-mod-php7.4 (7.4.16-1ubuntu2.1) ...
Processing triggers for php7.4-cli (7.4.16-1ubuntu2.1) ...
kumagai@tubasan:~/Develop/composer-project$ php composer.phar require geoip2/geoip2:~2.0 guzzle/guzzle:3.0
./composer.json has been updated
Running composer update geoip2/geoip2 guzzle/guzzle
Loading composer repositories with package information
Updating dependencies
Lock file operations: 7 installs, 0 updates, 0 removals
  - Locking cakephp/chronos (2.2.0)
  - Locking composer/ca-bundle (1.2.10)
  - Locking geoip2/geoip2 (v2.11.0)
  - Locking guzzle/guzzle (v3.0.0)
  - Locking maxmind-db/reader (v1.10.1)
  - Locking maxmind/web-service-common (v0.8.1)
  - Locking symfony/event-dispatcher (v2.1.13)
Writing lock file
Installing dependencies from lock file (including require-dev)
Package operations: 7 installs, 0 updates, 0 removals
  - Downloading composer/ca-bundle (1.2.10)
  - Downloading maxmind/web-service-common (v0.8.1)
  - Downloading maxmind-db/reader (v1.10.1)
  - Downloading geoip2/geoip2 (v2.11.0)
  - Downloading symfony/event-dispatcher (v2.1.13)
  - Downloading guzzle/guzzle (v3.0.0)
  - Installing cakephp/chronos (2.2.0): Extracting archive
  - Installing composer/ca-bundle (1.2.10): Extracting archive
  - Installing maxmind/web-service-common (v0.8.1): Extracting archive
  - Installing maxmind-db/reader (v1.10.1): Extracting archive
  - Installing geoip2/geoip2 (v2.11.0): Extracting archive
  - Installing symfony/event-dispatcher (v2.1.13): Extracting archive
  - Installing guzzle/guzzle (v3.0.0): Extracting archive
5 package suggestions were added by new dependencies, use `composer suggest` to see details.
Package guzzle/guzzle is abandoned, you should avoid using it. Use guzzlehttp/guzzle instead.
Generating autoload files
1 package you are using is looking for funding.
Use the `composer fund` command to find out more!

curl -sS https://getcomposer.org/installer | php
php composer.phar require geoip2/geoip2:~2.0 guzzle/guzzle:3.0
```

