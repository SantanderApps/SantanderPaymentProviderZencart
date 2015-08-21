# Install the module
## Before installation
* Make sure that you have an working Zen Cart installation.
* Make sure you have FTP access to the server where you have installed Zen Cart.

## Requirements
The following requirements must be fulfilled for this module to work.
* PHP version 5.3.0 or greater.
* PHP SoapClient ([http://php.net/manual/en/class.soapclient.php](http://php.net/manual/en/class.soapclient.php))
* Openssl
* cURL lib must be enabled for PHP ([http://php.net/manual/en/book.curl.php](http://php.net/manual/en/book.curl.php))
* libxml [http://php.net/manual/en/book.libxml.php](http://php.net/manual/en/book.libxml.php)

## Installation
* Upload ./extras/santander to the corresponding path of your Zen Cart environment and make sure that extras/santander/src/runtime is writeable by the server (file permission 775).
* Upload ./santander.php to the root folder of your Zen Cart installation.
* Upload ./includes/modules/payment/santander_loan.php to the corresponding path of your Zen Cart environment.
* Upload ./includes/modules/payment/santander to the corresponding path of your Zen Cart environment and make sure that the folder is writeable by the server (file permission 775).
* Upload ./includes/languages/english/modules/payment/santander_loan.php to the corresponding path of your Zen Cart environment.
* Upload ./includes/languages/swedish/modules/payment/santander_loan.php to the corresponding path of your Zen Cart environment.
* Go to the shop administration -> Modules -> Payment.
* Select "Santander Consumer Bank"
* Click on "install".
* Fill out the configuration form and then click "Save".

## Configuration parameters
* **Enable Santander Consumer Bank module:** whether to enable or disable the payment module.
* **Sort order of display:** specify the order the module will be disabled in the checkout.
* **Set Order Status:** select you preferred order status for orders paid with this payment module.
* **Payment Zone:** if a zone is selected, only enable this payment method for that zone.
* **Set Module Environment:** select which environment you want to run the module. Sandbox (test environment) is used for evaluating the module.
* **Store ID:** type the store ID that have been provided for you by Santander. This field will be automatically filled out when the module environment is set to "sandbox (test environment)".
* **Username:** type the username that have been provided for you by Santander. This field will be automatically filled out when the module environment is set to "sandbox (test environment)".
* **Password:** type the password that have been provided for you by Santander. This field will be automatically filled out when the module environment is set to "sandbox (test environment)".
* **Certificate:** (optional in sandbox/test environment) type the name of the file for the .pem certificate file that have been provided for you by Santander. This field will be automatically filled out when the module environment is set to "sandbox (test environment)".

* **Merchant ID:** (optional in sandbox/test environment) type the merchant ID that have been provided for you by your payment service provider. See list below for supported payment service providers.

## Supported payment service providers
Santander supports the following payment service providers:
* Dibs
* DebiTech o Nets
* Payex
* Samport