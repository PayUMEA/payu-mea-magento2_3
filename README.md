# PayU MEA Magento 2.3 extension #

This guide details how to install the PayU MEA Magento v2.3 extension

## Prerequisites
* Magento 2.3 installed application
* SSH access

## Dependencies

The extension requires the following extension in order to work properly:

- [`soap`](https://php.net/manual/en/book.soap.php)
- [`json`](https://php.net/manual/en/book.json.php)

## Installation

1) Download newest version of plugin from GitHub repository
2) Unpack the downloaded archive
3) Copy the files from "payu-mea-magento2-master" folder to your Magento 2 entity to folder \app\code\PayU\EasyPlus\. If such directory/path doesn't exist you will need to create it

After copyting the files you need to enable the extension by excuting the following command:
```bash
bin/magento module:enable --clear-static-content PayU_EasyPlus
bin/magento setup:upgrade
bin/magento cache:clean
```

## Configuration
To configure the extension, you have to navigate to **Stores > Configuration > Sales > Payment Methods** and find PayU 
extension listed among other payment methods

### Who do I talk to if I run into any issue? ###

* Just send an email to **support@payu.co.za** or open an issue using the issue tracker
