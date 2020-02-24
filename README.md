Codelicia\NyanCat
=================

Fork from the amazing work of @whatthejeff!

## Requirements

The Nyan Cat result printer for PHPUnit requires:

 * PHP 7.4+.
 * PHPUnit 9+.
 * A terminal emulator with support for ANSI escape sequences, including color
   and cursor control.

## Installation

The recommended way to install the Nyan Cat result printer for PHPUnit is
[through composer](http://getcomposer.org). Just create a `composer.json` file
and run the `composer install` command to install it:

~~~json
{
    "require-dev": {
        "codelicia/nyancat": "^2.0"
    }
}
~~~

Once installed, add the following attributes to the `<phpunit>` element in your
`phpunit.xml` file:

    printerFile="vendor/codelicia/nyancat/src/NyanCatPrinter.php"
    printerClass="Codelicia\NyanCat\NyanCatPrinter"

**NOTE:** If PHPUnit was not installed via composer, you also need to include
the composer autoloader. One easy way to do this is to add the following
attribute to the `<phpunit>` element in your `phpunit.xml` file:

    bootstrap="vendor/autoload.php"

## License

The Nyan Cat result printer for PHPUnit is licensed under the [MIT license](LICENSE).
