Message Lab
===========

> A Drupal 8 site for DTA Communications.

# Contents

* [What this is](#what-this-is)
* [How to use](#how-to-use)
* [Modules](#modules)
* [Themes](#themes)
* [License](#license)
-----------------------------------------
# What this is

This repository installs the code to build a Drupal 8 shell site meeting the dependency requirements of the DTA's "Message Lab".

Note it does not create content types, views or roles by default. These can be installed using the configuration API.

# How to use

The site is installed and managed with [Composer](https://getcomposer.org/). This includes all site dependencies, including core, modules and themes.

## Install Composer

Use Homebrew to install composer:
1. Install [Homebrew](https://brew.sh/).
2. Install Composer with the following commands:
  * `brew update`
  * `brew tap homebrew/dupes`
  * `brew tap homebrew/php`
  * `brew install php56` or `brew install php71` for PHP7.
  * `brew install composer`
3. Test the installation with `$ composer -v`.

## Install dependencies
Use Composer to install the dependencies. These are listed in the `composer.json` file:

`composer install`

## Install or update dependencies
Use Composer to install dependencies or to update existing dependencies.

To add modules or themes from [drupal.org](https://drupal.org), use the `drupal/` prefix for module names:

`composer require drupal/<module_name>`

It is a good idea to specify the version to better manage dependencies:

`composer require drupal/<module_name>:<version>`

For example, to install the latest version of Ctools, use the following command:

`composer require drupal/ctools:3.0`

For further information on managing Drupal sites using Composer, please see [*Using Composer to manage Drupal site dependencies*](https://www.drupal.org/docs/develop/using-composer/using-composer-to-manage-drupal-site-dependencies).

# Modules

The site has these module dependencies:
* [Module Filter (3.0)](https://drupal.org/project/module_filter)
* [Administration Toolbar (1.19)](https://drupal.org/project/admin_toolbar)
* [Backup and Migrate (4.x-dev)](https://drupal.org/project/backup_migrate)
* [Devel (1.0-rc)](https://drupal.org/project/devel)
* [Display Suite (3.1)](https://drupal.org/project/ds)
* [Pathauto (1.0)](https://drupal.org/project/pathauto)
* [Link CSS (1.x-dev)](https://www.drupal.org/project/link_css)
* [Easy Breadcrumbs (1.6)](https://www.drupal.org/project/easy_breadcrumb)

# Themes

The site has these theme dependencies:
* [Adminimal Theme (1.3)](https://drupal.org/project/adminimal_theme)
* [Message Lab Theme](https://github.com/govau/message-lab-theme)

# License

Copyright (c) Commonwealth of Australia. Licensed under [MIT](https://raw.githubusercontent.com/govau/uikit/master/LICENSE).
