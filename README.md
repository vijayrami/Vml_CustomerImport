# Vml_CustomerImport
Import Customer with cron command in CSV or JSON format

# Magento2 Module Vml CustomerImport

    ``vml/magento2-module-customerimport``

 - [Main Functionalities](#markdown-header-main-functionalities)
 - [Installation](#markdown-header-installation)
 - [Configuration](#markdown-header-configuration)
 - [Specifications](#markdown-header-specifications)
 - [Attributes](#markdown-header-attributes)


## Main Functionalities
Import Customer with cron command which is supplied via CSV or JSON format.

### Type 1: Zip file

 - Unzip the zip file in `app/code/Vml/CustomerImport`
 - Enable the module by running `php bin/magento module:enable Vml_CustomerImport`
 - Run Magento commands by running
   `php bin/magento set:upg && php bin/magento set:d:c && php bin/magento set:s:d -f && php bin/magento c:c && php bin/magento c:f`
 - Give `var` and `pub` folder to 777 permission by running `chmmod -R 0777 var/ pub/`

### Type 2: Composer

 - Make the module available in a composer repository for example:
    - private repository `repo.magento.com`
    - public repository `packagist.org`
    - public github repository as vcs
 - Add the composer repository to the configuration by running `composer config repositories.repo.magento.com composer https://repo.magento.com/`
 - Install the module composer by running `composer require magelearn/module-customform`
 - enable the module by running `php bin/magento module:enable Magelearn_Customform`
 - apply database updates by running `php bin/magento setup:upgrade`\*
 - Flush the cache by running `php bin/magento cache:flush`


## Configuration

- Front end URLs:
    - for customform: `/customform/`
    - for customform list page `/customform/index/list`
    - for customform view page `/customform/index/view/id/**`


## Specifications




## Attributes

