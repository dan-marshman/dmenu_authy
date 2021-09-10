# dmenu_authy
A simple wrapper to pipe authy data into dmenu, and then extract a temporaty token back out.

## Installation and Usage

### Installation
To install, close this repository or just save the dm-authy

### Dependencies
You will also require two dependencies
1. [xclip](https://archlinux.org/packages/extra/x86_64/xclip/)
2. [Mambembe](https://github.com/jaysonsantos/mambembe)

Obviously you also need dmenu. Presumably you won't be reading this page without it. 

### Setup
Register your device with Authy using the Mambembe instructions - currently:
```
mambembe-cli register-device --device-name <device-name> --phone <phone>
```
At the time of writing, Mambembe requires your phone number in the format e.g. XX-YYYYYYYY where XX is the country code.

### Usage
Simply call `dm-authy`.  It will pipe all your accounts into dmenu - choose one and your token and it will be copied to clipboard.

### Warning
Exercise some caution with this - it is not an official client. As an example, Authy may temporarily (I think) suspend your account if you use it repeatedly (e.g. several times a minute)
