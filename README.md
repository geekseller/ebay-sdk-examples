This project contains several examples of using the [eBay SDK for PHP](https://github.com/geekseller/ebay-sdk-php).

# About this repository

This repository is maintained by the company [GeekSeller.com](https://www.geekseller.com/), and it is a fork of another [EBAY-SDK-EXAMPLES](https://github.com/davidtsadler/ebay-sdk-examples). The original code has been developed by [David T. Sadler](https://github.com/davidtsadler), however, in February 2020, David archived the project and decided not to continue maintaining it. GeekSeller uses David’s SDK in the production, so we decided to create a fork of this SDK, maintain it as a separate project and offer it to the community.

Please note that GeekSeller is part of the eBay Developer Program and we have our eBay application listed in the [eBay Solution Directory](https://cgi6.ebay.com/ws/eBayISAPI.dll?SolutionsDirectory&page=details&solutionId=705084376), however, this SDK is not endorsed, sponsored or maintained by eBay.


## Requirements

  - PHP 5.3.3 or greater with the following extensions:
    - cURL
    - libxml
  - SSL enabled on the cURL extension so that https requests can be made.

## Installation

1. Download the project.

   ```
   git clone https://github.com/geekseller/ebay-sdk-examples.git
   ```

1. From the `ebay-sdk-examples` directory install Composer with:

   ```
   curl -sS https://getcomposer.org/installer | php
   ```

1. Install the dependencies.

   ```
   php composer.phar install
   ```

## Configuration

All the examples load configuration settings from a `configuration.php` file located in the root of the project directory. This file can be created by running the following command inside the `ebay-sdk-examples` directory:

   ```
   cp configuration.php.example configuration.php
   ```

Edit the resulting `configuration.php` file and specify your eBay application keys. Ensure that you enter values for both the sandbox and production enviroments.

**Be careful not to commit the `configuration.php` file into an SCM repository as you risk exposing your eBay application keys to more people than intended.**

## Examples

There are several examples for each service that the SDK supports and they are listed in the `README` file for each service.

1. [Finding](https://github.com/geekseller/ebay-sdk-examples/blob/master/finding/README.md)

1. [Trading](https://github.com/geekseller/ebay-sdk-examples/blob/master/trading/README.md)

1. [Shopping](https://github.com/geekseller/ebay-sdk-examples/blob/master/shopping/README.md)

1. [Business Policies Management](https://github.com/geekseller/ebay-sdk-examples/blob/master/business-policies-management/README.md)

1. [Large Merchange Services](https://github.com/geekseller/ebay-sdk-examples/blob/master/large-merchant-services/README.md)

1. [Half Finding](https://github.com/geekseller/ebay-sdk-examples/blob/master/half-finding/README.md)

1. [Resolution Case Management](https://github.com/geekseller/ebay-sdk-examples/blob/master/resolution-case-management/README.md)

1. [Return Management](https://github.com/geekseller/ebay-sdk-examples/blob/master/return-management/README.md)

1. [Misc](https://github.com/geekseller/ebay-sdk-examples/blob/master/misc/README.md)

1. [Async](https://github.com/geekseller/ebay-sdk-examples/blob/master/async/README.md)

1. [Account](https://github.com/geekseller/ebay-sdk-examples/blob/master/account/README.md)

1. [Inventory](https://github.com/geekseller/ebay-sdk-examples/blob/master/inventory/README.md)

1. [Product](https://github.com/geekseller/ebay-sdk-examples/blob/master/product/README.md)

1. [Product Metadata](https://github.com/geekseller/ebay-sdk-examples/blob/master/product_metadata/README.md)

1. [Browse](https://github.com/geekseller/ebay-sdk-examples/blob/master/browse/README.md)

1. [Analytics](https://github.com/geekseller/ebay-sdk-examples/blob/master/analytics/README.md)

1. [OAuth Tokens](https://github.com/geekseller/ebay-sdk-examples/blob/master/oauth-tokens/README.md)

1. [Taxonomy](https://github.com/geekseller/ebay-sdk-examples/blob/master/taxonomy/README.md)

1. [Feed](https://github.com/geekseller/ebay-sdk-examples/blob/master/feed/README.md)

1. [Metadata](https://github.com/geekseller/ebay-sdk-examples/blob/master/metadata/README.md)

1. [Catalog](https://github.com/geekseller/ebay-sdk-examples/blob/catalog/metadata/README.md)

1. [Complicance](https://github.com/geekseller/ebay-sdk-examples/blob/compliance/metadata/README.md)

To run an example from the command line use the `php` command followed by the name of the example file.

```
php finding/01-simple-keywords-search.php
```
