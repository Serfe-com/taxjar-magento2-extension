<img src=docs/serfe.png width=100 align="right"/>

# Serfe TaxJar Magento 2 Extension  

[![Latest Stable Version](https://poser.pugx.org/serfe/magento2-taxjar/version)](https://packagist.org/packages/serfe/magento2-taxjar)  

The **Serfe TaxJar Magento 2 Extension** is a fork of the [official TaxJar Magento 2 module (v2.2.0)](https://github.com/taxjar/taxjar-magento2-extension). This extension integrates seamlessly with [TaxJar](http://www.taxjar.com) to provide real-time sales tax calculations and zip-based backup rates.  

## Why This Fork?  

The official TaxJar Magento 2 extension has not been updated since **2022**, leading to compatibility issues with newer Magento versions. Our fork was created to:  

- **Ensure ongoing compatibility** with the latest Magento 2 releases and PHP versions.  
- **Fix known issues** reported in the original repository that remain unresolved.  
- **Provide active maintenance** for merchants relying on TaxJar for tax calculations.  
- **Enable community contributions**, allowing faster issue resolution and feature improvements.  

By keeping this module updated, we help Magento store owners avoid potential tax calculation errors and maintain compliance with evolving tax regulations.  

## Key Features  

- **Real-Time Tax Calculation**: Automatically calculates sales tax during checkout using TaxJar's API.  
- **Zip-Based Backup Rates**: Ensures tax accuracy even if live API calls fail.  
- **Seamless Magento Integration**: Compatible with Magento's native tax configuration.  
- **Enhanced Maintenance & Support**: Actively maintained by [Serfe](https://www.serfe.com/).  

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

To configure the extension, go to **Stores > Configuration > Sales > TaxJar** and enter your **TaxJar API token**. Follow the official [TaxJar Magento 2 Guide](https://developers.taxjar.com/integrations/guides/magento2/) for detailed setup instructions.  

## Running Tests  

To run integration tests for checkout calculations, clone the repository into your Magento 2 instance. You'll need an active TaxJar API token (preferably a test account).  

```bash
git clone https://github.com/serfe/magento2-taxjar.git app/code/Serfe/TaxJar
```  

Then, follow the setup instructions to run PHPUnit tests.  

## About This Fork  

This module is a **fork of the official TaxJar Magento 2 extension (v2.2.0)**, which has not received updates since 2022. Our fork provides essential updates, bug fixes, and ongoing maintenance to ensure full compatibility with newer Magento versions.  

### **Differences from the Official Module**  

| Feature | Official TaxJar Module | Serfe TaxJar Fork |
|---------|----------------------|-------------------|
| **Magento 2 Compatibility** | Up to Magento 2.4.3 | Magento 2.4.7+ |
| **PHP Support** | PHP 7.4 (deprecated) | PHP 8.2+ |
| **Bug Fixes & Improvements** | No recent updates | Actively maintained |
| **Community Contributions** | Abandoned | Open to contributions |

## About Us  

[Serfe](https://www.serfe.com/?utm_medium=referral_profile&utm_source=github&utm_campaign=115959) specializes in e-commerce solutions for Magento 2, focusing on performance, scalability, and usability. Visit our website for more details.  

## Contributing  

We welcome contributions! To contribute, fork this repository, make your changes, and submit a pull request.  

---

<sub>Inspired by the official [TaxJar Magento 2 extension](https://github.com/taxjar/taxjar-magento2-extension).</sub>  
