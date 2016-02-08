# Installation

    vagrant init johnstyle/localserver
    vagrant plugin install vagrant-vbguest
    vagrant up

# Connections

## SSH

    vagrant ssh

- shh root    : toor
- ssh vagrant : vagrant

## HTTP

Edit host file and add 

    192.168.56.101  localhost.vm            www.localhost.vm
    192.168.56.101  wordpress-4.x.vm        www.wordpress-4.x.vm
    192.168.56.101  wordpress-3.x.vm        www.wordpress-3.x.vm
    192.168.56.101  prestashop-1.7.x.vm     www.prestashop-1.7.x.vm
    192.168.56.101  prestashop-1.6.x.vm     www.prestashop-1.6.x.vm
    192.168.56.101  prestashop-1.5.x.vm     www.prestashop-1.5.x.vm
    192.168.56.101  prestashop-1.4.x.vm     www.prestashop-1.4.x.vm
    192.168.56.101  magento-2.x.vm          www.magento-2.x.vm
    192.168.56.101  drupal-8.x.vm           www.drupal-8.x.vm
    192.168.56.101  nodejs-app.vm
    192.168.56.101  symfony-app.vm
    
Got to:

    http://localhost.vm

# Starter kits

## Wordpress

- http://wordpress-4.x.vm/
- http://wordpress-3.x.vm/

## Prestashop

- http://prestashop-1.7.x.vm/
- http://prestashop-1.6.x.vm/
- http://prestashop-1.5.x.vm/install-dev/
- http://prestashop-1.4.x.vm/install-dev/

## Magento

- http://magento-2.x.vm/

## Drupal

- http://drupal-8.x.vm/

## Symfony-app

    php bin/console server:run
    
- http://symfony-app.vm/

## Nodejs-app

    node app.js
    
- http://nodejs-app.vm/

# Databases

## MySql (mariadb)

Databases names are same of vhost, example: "prestashop-1.6.x.vm" as "prestashop-1.6.x"

Host: 192.168.56.101
Port: 3306
User: root 
Pass: toor

    mysql -p

## MongoDb

Host: 192.168.56.101
Port: 27017

    mongo

## Elasticsearch

Host: 192.168.56.101
Port: 9200
