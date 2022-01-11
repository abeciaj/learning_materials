# Mac Setup

## The quickest way to install php on macOS is with homebrew:

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

brew -v
```

## Installing PHP
Installing the latest version of PHP (v8.1)
```
brew install php
php -v
```
or installing a specific version of PHP using @
```
brew install php@7.4
php -v
```

# Ubuntu Setup

## Enabling PHP Repository
Ondřej Surý, a Debian developer, maintains a repository that includes multiple PHP versions. To enable the repository , run:
```
sudo apt install software-properties-common
sudo add-apt-repository ppa:ondrej/php
```
## Installing PHP
```
sudo apt update
sudo apt install php7.4
php -v
```

# Windows Setup
## 1. Download the PHP File
Download the PHP zip file [Here.](https://www.php.net/downloads.php)

## 2. Extract the Files
Create a new `php` folder in the root of your `C:\` drive and extract the contents of the ZIP into it.

PHP can be installed anywhere on your system, but you’ll need to change the paths referenced below if `C:\php` isn’t used.

## 3. Configure php.ini
PHP’s configuration file is named `php.ini`. This doesn’t exist initially, so copy `C:\php\php.ini-development` to `C:\php\php.ini`. This default configuration provides a development setup which reports all PHP errors and warnings.

There are several lines you may need to change in a text editor (use search to find the current value). In most cases, you’ll need to remove a leading semicolon (`;`) to uncomment a setting.

First, enable any required extensions. This will depend on the libraries you want to use, but the following extensions should be suitable for most applications:

```
extension=curl
extension=gd
extension=mbstring
extension=pdo_mysql
```

## 4. Add C:\php to the path environment variable
To ensure Windows can find the PHP executable, you need to change the `PATH` environment variable. Click the Windows Start button and type *“environment”*, then click **Edit the system environment variables**. Select the **Advanced** tab, and click the **Environment Variables** button.

Scroll down the **System variables** list and click **Path** followed by the **Edit** button. Click **New** and add `C:\php`: