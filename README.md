# Drupal 8 configuration/migration notes


### Style Extensions

Civicrm Menu > Administer > System Settings > Resource URLs

Add url https://northbridgetech.org/apps/waterwheel/module/core/style/civicrm.css to the Custom CSS URL field. (This file is managed inside the waterwheel repository.)

To: core/themes/bartik/css/base/elements.css

Add at top: @import url("https://northbridgetech.org/apps/waterwheel/module/core/style/civicrm.css");

? Put Font Awesome library at sites/all/libraries/fontawesome

# Configuration/migration notes

## Views
Don't forget to update Drupal settings.php in order to pull in all custom fields

Get the database mappings from CiviCRM here: http://northbridgetech.org/dev/members/index.php?q=civicrm/admin/setting/uf&reset=1

instructions: https://wiki.civicrm.org/confluence/display/CRMDOC41/Views3+Integration

## Code Customizations
Confirm.tpl and ThankYou.tpl at  
sites/all/modules/civicrm/templates/CRM/Contribute/Form/Contribution

"the contribution" => "your membership registration"

"To complete this transaction" => "To complete"

"Your transaction will not be completed" => "Your submission will not be completed"

"Your transaction" => "Your submission"

(Will have to re-do with any code upgrade.)

Formilla: Add inclusion script and title substitution scripts to modules/system/html.tpl.php

Tweak Booking extension: Comment these lines at sites/default/files/civicrm/ext/uk.co.compucorp.civicrm.booking/CRM/Admin/Form/*.php 

`// protected $_id = NULL;`
`// protected $_sid = NULL;`


### Style Extensions

Administer > System Settings > Resource URLs

Add url https://northbridgetech.org/apps/waterwheel/module/core/style/civicrm.css to the Custom CSS URL field. (This file is managed inside the waterwheel repository.)

To: themes/bartik/css/style.css

Add at top: @import url("https://northbridgetech.org/apps/waterwheel/module/core/style/civicrm.css");

Put Font Awesome library at sites/all/libraries/fontawesome

## CiviCRM Errors

`public_html/apps/members/sites/default/files/civicrm/ConfigAndLog`

## Drupal Errors

Admin > Reports > Recent Log Messages

OR

add output directives to apps/members/index.php

Also see:

https://www.drupal.org/forum/support/post-installation/2010-05-18/logfiles-of-a-drupal-site

https://www.drupal.org/project/error_log

