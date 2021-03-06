# CKEditor plugin LineUtils Bundle for Symfony2
Symfony2 Bundle to integrate the CKEditor plugin LineUtils

## Current Version

LineUtils v4.5.1

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "stinger/ckeditor-lineutils-bundle": "~4.5.1"
    }
}
```

### Add bundle to your application kernel

``` php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Stinger\CKEditorLineUtilsBundle\StingerCKEditorLineUtilsBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update stinger/ckeditor-lineutils-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ php app/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ php app/console assets:install --symlink web
```

### Usage

``` yaml
trsteel_ckeditor:
    external_plugins:
      lineutils:
        path: 'bundles/stingerckeditorlineutils'
```



# Licenses

Refer to the source code of the included files for license information

# References

1. http://ckeditor.com/addon/lineutils
2. http://symfony.com
