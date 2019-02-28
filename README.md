# recurreportpayproc

This applies two CiviCRM core patches to enable "payment_processor_id" on the recurring contributions report.

The extension is licensed under [AGPL-3.0](LICENSE.txt).

## Requirements

* PHP v7.0+
* CiviCRM 5.10.3 or 5.10.4

## Installation

This extension should only be installed by developers after evaluating the files that it overrides:
* CRM/Contribute/BAO/ContributionRecur.php
* CRM/Contribute/DAO/ContributionRecur.php
* CRM/Report/Form/Contribute/Recur.php
* xml/schema/Contribute/ContributionRecur.xml

## Patches

* Add pseudoconstant for payment_processor_id to contributionrecur https://github.com/civicrm/civicrm-core/pull/13702
* Add payment_processor column/filter to recurring contribution report https://github.com/civicrm/civicrm-core/pull/13699
