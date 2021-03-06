# Magento 2 Mailgun Module

[![Latest Stable Version](https://poser.pugx.org/bogardo/mailgun-magento2/v/stable?format=flat-square)](https://packagist.org/packages/bogardo/mailgun-magento2)
[![Monthly Downloads](https://poser.pugx.org/bogardo/mailgun-magento2/d/monthly?format=flat-square)](https://packagist.org/packages/bogardo/mailgun-magento2)
[![License](https://poser.pugx.org/bogardo/mailgun-magento2/license?format=flat-square)](https://packagist.org/packages/bogardo/mailgun-magento2)

Send Magento's transactional e-mails with the [Mailgun API](http://www.mailgun.com/).

### Installation

Install using composer

```bash
composer require bogardo/mailgun-magento2
```

### Configuration

Module configuration can be found in:  `Stores -> Configuration -> Services -> Mailgun`

Fill in your Mailgun Domain and your API Keys.
These can be found in your [Mailgun control panel](https://mailgun.com/app/dashboard).

Next, enable the module by setting the `Enabled` option to `Yes`.

### Usage

All transactional email that are send by your Magento application are now send using the Mailgun API.
You can access the mail logs in your [Mailgun control panel](https://mailgun.com/app/logs).

## Changelog

#### 0.1.4
Fix version number

#### 0.1.3
Remove `extra.map` from composer.json.
Since the 2.0.0-RC version it is no longer needed as modules can now also be loaded from the vendor/ directory and don't need to be copied to the app/code directory.
([Source](http://magento.stackexchange.com/questions/93502/magento2-custom-module-downloaded-by-composer-at-two-places/93503#93503))

#### 0.1.2
- Add correct license
- Add badges to readme

#### 0.1.1
- Update README
    - Add installation instructions
    - Add changelog

#### 0.1.0
- Base Module
- Test Mode
- Debug Mode: Send messages to [Mailgun's Postbin](http://bin.mailgun.net/)
