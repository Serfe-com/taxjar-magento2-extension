<img src=docs/serfe.png width=200 align="right"/>

# Serfe TaxJar Magento 2 Extension

[![Latest Stable Version](https://poser.pugx.org/serfe/magento2-taxjar/version)](https://packagist.org/packages/serfe/magento2-taxjar)

The **Serfe TaxJar Magento 2 Extension** is a fork of the [official TaxJar Magento 2 module (v2.2.0)](https://github.com/taxjar/taxjar-magento2-extension). This extension integrates seamlessly with [TaxJar](http://www.taxjar.com) to provide real-time sales tax calculations and zip-based backup rates.

## Key Features

- **Real-Time Tax Calculation**: Automatically calculates sales tax during checkout using TaxJar's API.
- **Zip-Based Backup Rates**: Ensures tax accuracy even if live API calls fail.
- **Seamless Magento Integration**: Compatible with Magento's native tax configuration.
- **Enhanced Maintenance & Support**: Updated and maintained by [Serfe](https://www.serfe.com/).

## Installation Guide

### Install via Composer

Run the following command in your terminal:

```bash
composer require serfe/magento2-taxjar
```

### Enable and Set Up the Module

After installation, enable and configure the module using Magento CLI:

```bash
bin/magento module:enable Serfe_TaxJar
bin/magento setup:upgrade
bin/magento setup:di:compile
bin/magento cache:clean
```

## Configuration

To configure the extension, go to **Stores > Configuration > Sales > TaxJar** and enter your **TaxJar API token**. Follow the official [TaxJar Magento 2 Guide](http://www.taxjar.com/guides/integrations/magento2/) for detailed setup instructions.

## Running Tests

To run integration tests for checkout calculations, clone the repository into your Magento 2 instance. You'll need an active TaxJar API token (preferably a test account).

```bash
git clone https://github.com/serfe/magento2-taxjar.git app/code/Serfe/TaxJar
```

Then, follow the setup instructions to run PHPUnit tests.

## About This Fork

This module is a **fork of the official TaxJar Magento 2 extension (v2.2.0)**. The original repository can be found at [GitHub - TaxJar Magento 2 Extension](https://github.com/taxjar/taxjar-magento2-extension). Our fork includes maintenance updates and improvements for better compatibility with newer Magento versions.

## About Us

[Serfe](https://www.serfe.com/?utm_medium=referral_profile&utm_source=github&utm_campaign=115959) specializes in e-commerce solutions for Magento 2, focusing on performance, scalability, and usability. Visit our website for more details.

## Contributing

We welcome contributions! To contribute, fork this repository, make your changes, and submit a pull request.

---

<sub>Inspired by the official [TaxJar Magento 2 extension](https://github.com/taxjar/taxjar-magento2-extension).</sub>
