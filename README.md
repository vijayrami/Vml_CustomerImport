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

## Specifications




## Attributes

