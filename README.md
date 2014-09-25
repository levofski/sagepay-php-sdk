sagepay-php-sdk
===============

Official Sage Pay PHP SDK for server and direct integrations

This repo takes the official Sage Pay V3 PHP SDK and turns it into a composer compatible include for use with modern frameworks. No code has been modified from the existing Sage Pay code so it allows you to build your own wrappers for your integration.

Installation
------------

To install this library to your project it is recommended to use composer. There is a composer archieve at:
https://packagist.org/packages/alvsystems/sagepay-php-sdk

To include the library in your project just add the following line to your require directive in your composer.json file:

<code>"alvsystems/sagepay-php-sdk": "0.1.*"</code> or
<code>"alvsystems/sagepay-php-sdk": "0.1.*@dev"</code> for the latest development build.

then run:

<code>php composer.phar install</code> or <code>php composer.phar update</code>

Install Composer
----------------

Run this in your terminal to get the latest Composer version:

<code>curl -sS https://getcomposer.org/installer | php</code>
Or if you don't have curl:
<code>php -r "readfile('https://getcomposer.org/installer');" | php</code>

This installer script will simply check some php.ini settings, warn you if they are set incorrectly, and then download the latest composer.phar in the current directory

Usage
-----

The Official SagePay SDK does not currently use namespaces so to use the SDK you simply run commands such as:
<code>
$api = SagepayApiFactory::create('SERVER', $config);
$api->setBasket($basket);
</code>

There is a working demo if you download the official SagePay PHP SDK at: http://www.sagepay.co.uk/support/find-an-integration-document/server-integration-documents

Updates
-------

I couldn't find any versioning info for the SagePay PHP SDK so please check yourself if you think this archive may be out of date or better yet you can make a request to update this repo yourself!

Copyright
---------

The SDK belongs to SagePay and is their intellectual property. No license information is available but this is a publicly accessible source code. I do not intend any copyright infringement and am simply creating a wrapper to aid developers (including myself) to use the SagePay SDK in their composer compatible projects.

Contact
-------

If you need to contact me you can get in touch with me via my website: http://www.alvinchevolleaux.com
