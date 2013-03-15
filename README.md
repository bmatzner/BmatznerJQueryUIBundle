# jQuery UI Bundle for Symfony2

## Current Version

jQuery UI v1.10.2

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
        // ...
        "bmatzner/jquery-ui-bundle": "*"
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
        new Bmatzner\JQueryUIBundle\BmatznerJQueryUIBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update bmatzner/jquery-ui-bundle
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

## Usage

Load a jQuery UI theme, for instance one of the included default themes

``` html
<link rel="stylesheet" type="text/css" href="{{ asset('bundles/bmatznerjqueryui/css/smoothness/jquery-ui.css') }}" />
<link rel="stylesheet" type="text/css" href="{{ asset('bundles/bmatznerjqueryui/css/smoothness/jquery.ui.theme.css') }}" />
```

Load jQuery and jQuery UI

``` html
<script type="text/javascript" src="{{ asset('bundles/bmatznerjquery/js/jquery.min.js') }}"></script>
<script type="text/javascript" src="{{ asset('bundles/bmatznerjqueryui/js/minified/jquery-ui.min.js') }}"></script>
```

## Licenses

Refer to the source code of the included files for license information

## References

1. http://jqueryui.com
2. http://symfony.com
