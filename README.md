# Vml_CustomerImport
Import Customer with cron command in CSV or JSON format

# Magento2 Module Vml CustomerImport

    ``vml/magento2-module-customerimport``

 - [Main Functionalities](#main-functionalities)
 - [Installation](#installation)
 - [Features](#features)
 - [Configurations](#configurations)
 - [Screenshots](#screenshots)


## Main Functionalities
Import Customer with cron command which is supplied via CSV or JSON format.

## Installation
### Type 1: Zip file

 - Unzip the zip file in `app/code/Vml/CustomerImport`
 - Enable the module by running `php bin/magento module:enable Vml_CustomerImport`
 - Run Magento commands by running

   `php bin/magento set:upg && php bin/magento set:d:c && php bin/magento set:s:d -f && php bin/magento c:c && php bin/magento c:f`
 - Give `var` and `pub` folder to 777 permission by running `chmmod -R 0777 var/ pub/`

### Type 2: Composer

 - Install the module composer by running `composer require vml/magento2-module-customerimport`
 - Enable the module by running `php bin/magento module:enable Vml_CustomerImport`
 - Run Magento commands by running

   `php bin/magento set:upg && php bin/magento set:d:c && php bin/magento set:s:d -f && php bin/magento c:c && php bin/magento c:f`
 - Give `var` and `pub` folder to 777 permission by running `chmmod -R 0777 var/ pub/`


## Features

Create customers from CSV or JSON file from command line terminal.

## Configurations

`bin/magento customer:import <profile-name> <source>`

#### So to import from the CSV and the JSON respectively the user would execute either one of the following

##### profile-name is 'sample-csv' or 'sample-json'

##### source is your file path name added in `var/import` folder (eg. 'sample.csv' or 'sample.json')

     *   [-f|--customer-firstname CUSTOMER-FIRSTNAME]
     *   [-l|--customer-lastname CUSTOMER-LASTNAME]
     *   [-e|--customer-email CUSTOMER-EMAIL]
     *   [-p|--customer-password CUSTOMER-PASSWORD]
     *   [-w|--website WEBSITE]
     *   [-s|--send-email [SEND-EMAIL]]
     *   [-ns|--newsletter-subscribe [NEWSLETTER-SUBSCRIBE]]
     *
    php bin/magento magelearn:customer:create -f "Vijay" -l "Rami" -e "vijaymrami@gmail.com" -p "test123" -w 1
    php bin/magento magelearn:customer:create -f "Vijay" -l "Rami" -e "vijaymrami@gmail.com" -p "test123" -w 1 -s 1 --newsletter-subscribe 1


## Screenshots

