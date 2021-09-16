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


