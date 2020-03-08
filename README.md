# CakePHP 2 Multiple Apps Same Core Valet Driver
Add CakePHP 2 with multiple apps and one core support to Laravel Valet

## Installation

This driver allows you to have several apps using the same CakePHP library.

Installation
1. Copy the file [`CakePHP2MultipleAppsSameCoreValetDriver.php`](CakePHP2MultipleAppsSameCoreValetDriver.php) to your Valet Drivers folder located at `~/.valet/Drivers` .
2. Use the `link` command to point to each of the apps inside the CakePHP library.

##Example:
Suppose we have 3 apps within the root structure of the CakePHP directory as follows:


    . 							# CakePHP root directory
    ├── app						# First app
    │   ├── Plugin
    │   ├── Vendor
    │   ├── webroot
    │   └── ...
    ├── app2					# Second app
    │   ├── Plugin
    │   ├── Vendor
    │   ├── webroot
    │   └── ...
    ├── app3					# Third app
    │   ├── Plugin
    │   ├── Vendor
    │   ├── webroot
    │   └── ...
    ├── lib
    ├── Cake
    ├── plugins
    ├── vendors
    └── ...


Then the commands to be executed would be the following:
`cd ~/cakephp-installation/app/`

`valet link app1`

`cd ~/cakephp-installation/app2/`

`valet link app2`

`cd ~/cakephp-installation/app3/`

`valet link app3`

Done!

### Documentation
* Custom  [Laravel Valet](https://laravel.com/docs/7.x/valet) Driver for [CakePHP 2](https://book.cakephp.org/2.0/en/index.html).

## License
See the [LICENSE](LICENSE) file for more info.