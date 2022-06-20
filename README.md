# prn_api

Utility API Calls for the Parking Reform Network

* cv api PRN.importcharge ppid=(payment processor id) charge=(stripe charge id) contact_id=(contact id) financial_type_id=(financial type id)

The importcharge api in the [Stripe Extension for CiviCRM](https://lab.civicrm.org/extensions/stripe) doesn't work with one-off transactions that do not have a stripe invoice. This modified version hacks support for those transacations in. Use at your own risk.


The extension is licensed under [AGPL-3.0](LICENSE.txt).

## Requirements

* PHP v7.2+
* CiviCRM 5.5+

## Installation (Web UI)

Learn more about installing CiviCRM extensions in the [CiviCRM Sysadmin Guide](https://docs.civicrm.org/sysadmin/en/latest/customize/extensions/).

## Installation (CLI, Zip)

Sysadmins and developers may download the `.zip` file for this extension and
install it with the command-line tool [cv](https://github.com/civicrm/cv).

```bash
cd <extension-dir>
cv dl prn_api@https://github.com/FIXME/prn_api/archive/master.zip
```

## Installation (CLI, Git)

Sysadmins and developers may clone the [Git](https://en.wikipedia.org/wiki/Git) repo for this extension and
install it with the command-line tool [cv](https://github.com/civicrm/cv).

```bash
git clone https://github.com/FIXME/prn_api.git
cv en prn_api
```

## Known Issues

* No tests!
* financial_type lookup doesn't work, id required.

## Acknowledgement

Based on script in CiviCRM Stripe Extension https://lab.civicrm.org/extensions/stripe
