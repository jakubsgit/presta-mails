# Carry Mailing

Szablony maili dla sklepu internetowego Carry.

## Lista szablonów wykonanych i zatwierdzonych

### Priorytety

- [&check;] order_conf *
- [&check;] order_canceled *
- [&check;] order_changed
- [&check;] payment *
- [&check;] preparation *
- [&check;] shipped *
- [&check;] account
- [ ] password
- [&check;] password_query *

### Dodatkowe

- [&check;] account *
- [ ] cheque *
- [ ] contact *
- [ ] contact_form *
- [ ] outofstock *
- [ ] refund *
- [ ] reply_msg *
- [ ] textmail *


## Usage

During development, you just need to watch files:

`gulp watch`

This will detect changes on your files and output a compiled version in `./dist/en/`.  
3 languages are available during development but more languages are available when the emails are installed on PrestaShop. More information below.

## Build

To install the emails on PrestaShop, you need to build a package:

`gulp build`

This will create a zip file in `./dist/` with the name you set in the `./src/config/settings.json`.

To install the zip file that contains the emails, you need to use the Emails Manager available in the PrestaShop back office.
This is also this file you will need to submit on [PrestaShop Addons](https://addons.prestashop.com) if you want to sell it.
The emails are translated by the module during the installation and the dynamic variables & conditions are processed (see "Dynamic variables" and "Conditions" for more information).