# PHPNuxBill - PHP Mikrotik Billing

![PHPNuxBill](install/img/logo.png)

## Feature

- Voucher Generator and Print
- Self registration
- Multi Router Mikrotik
- Hotspot & PPPOE
- Easy Installation
- Multi Language
- Payment Gateway Midtrans, Xendit and Tripay
- SMS validation for login
- Whatsapp Notification to Consumer
- Telegram Notification for Admin

See [How it Works / Cara Kerja](https://github.com/hotspotbilling/phpnuxbill/wiki/How-It-Works---Cara-kerja)

## Payment Gateway And Plugin

- [Payment Gateway List](https://github.com/orgs/hotspotbilling/repositories?q=payment+gateway)
- [Plugin List](https://github.com/orgs/hotspotbilling/repositories?q=plugin)

You can download payment gateway and Plugin from Plugin Manager

## System Requirements

Most current web servers with PHP & MySQL installed will be capable of running PHPNuxBill

Minimum Requirements

- Linux or Windows OS
- PHP Version 7.2+
- Both PDO & MySQLi Support
- GD2 Image Library
- CURL support
- MySQL Version 4.1.x and above

can be Installed in Raspberry Pi Device.

The problem with windows is hard to set cronjob, better Linux

## Installation

### Git Clone

clone this repository or download zip or release

1. Rename **pages_template** to **pages**
2. Rename **config.sample.php** to **config.php** and make it writeable (chmod 777)
3. make writeable folder **ui/cache/** and **ui/compiled**
4. Open web and run installation
5. set [cronjob](https://github.com/hotspotbilling/phpnuxbill/wiki/Cron-Jobs) or scheduller for **system/cron.php**
6. make **config.php** unwriteable (chmod 644)

### Composer install

Go to directory you want to install
Install Composer in your system

```bash
# Debian/Ubuntu
sudo apt install composer
# Centos/Redhat
sudo yum install composer
```

install on curent directory

```bash
composer create-project hotspotbilling/phpnuxbill .
```

install on new directory

```bash
composer create-project hotspotbilling/phpnuxbill phpnuxbill
```

### Manual Installation

1. Download project from [Master Branch](https://github.com/hotspotbilling/phpnuxbill/archive/refs/heads/master.zip) or from [Release](https://github.com/hotspotbilling/phpnuxbill/releases)
2. unzip and upload it to server
3. Rename **pages_template** to **pages**
4. Rename **config.sample.php** to **config.php** and make it writeable (chmod 777)
5. make writeable folder **ui/cache/** and **ui/compiled**
6. Open web and run installation
7. set [cronjob](https://github.com/hotspotbilling/phpnuxbill/wiki/Cron-Jobs) or scheduller for **system/cron.php**
8. make **config.php** unwriteable (chmod 644)

### Docker installation

[see this repo](https://github.com/animegasan/phpnuxbill)

## UPDGRADE

for old version, below Version 6, backup **system/config.php**, delete all file except folder **pages**, upload all new files, put **config.php** in root folder (not in system folder), got to folder **/install** and run Update.

for version 6 above, just replace all files, using filezilla can choose overwrite if different file size or time.

or git pull if you use git clone

## RADIUS system

Still on development

## Technical Support

Start from Rp 500.000 or $50

If you chat me for any technical support, you need to pay, except for Donors, ask anything for free in the [discussion](/hotspotbilling/phpnuxbill/discussions) page

[Telegram](https://t.me/ibnux)

[Website](https://ibnux.net/layanan)

## License

GNU General Public License version 2 or later

see LICENSE file

## [CHANGELOG](CHANGELOG.md)

## Donate to ibnux

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://paypal.me/ibnux)

BCA: 5410454825

Mandiri: 163-000-1855-793

a.n Ibnu Maksum

## SPONSORS

- [mlink.id](https://mlink.id)
- [https://github.com/sonyinside](https://github.com/sonyinside)
