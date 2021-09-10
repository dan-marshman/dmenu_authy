# dmenu_authy
Simple wrapper to pipe authy data into dmenu, and the token for the chosen account back out

## Installation and Usage

### Installation
To install, close this repository or just save the dm-authy

You will also require two dependencies
1. [https://archlinux.org/packages/extra/x86_64/xclip/](xclip)
2. [https://github.com/jaysonsantos/mambembe](Mambembe)

Register your device with Authy using the Mambembe instructions - currently:
```
mambembe-cli register-device --device-name <device-name> --phone <phone>
```
At the time of writing, phone number needs to be in the format e.g. XX-YYYYYYYY where XX is the country code.

### Usage
Simply call `dm-authy`.  It will pipe all your accounts into dmenu - choose one and your token and it will be copied to clipboard.

### Warning
Be careful using this - it is not an official client. As an example, Authy may temporarily (I think) suspend your account if you use it repeatedly (e.g. several times a minute)
