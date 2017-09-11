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

### Style Extensions

/civicrm/admin/setting/url&reset=1

Add path to <waterwheel>/module/core/style/civicrm.css to the Custom CSS URL field. (This file is managed inside the waterwheel repository.)

To: themes/bartik/css/style.css

Add at top: @import url("http://northbridgetech.org/apps/waterwheel/module/core/style/civicrm.css");

Put Font Awesome library at sites/all/libraries/fontawesome

## Drupal Modules: 

See latest screen captures in this directory at modules*.png

Views 7.x.3.18  
Views Build Operations 7.x.3.4  
User Import 7.x.3.2  
Chaos 7.x.1.12  
Advanced Help 7.x.1.3    
Password Reset Landing Page 7.x.1.1  
Views Conditional 7.x.1.3  
Menu Items Visibility 7.x.1.0-beta2  
Rules 7.x.2.10  
Quiz 7.x.5.1  
Entity 7.x.1.8  
Token 7.x.1.7  
Libraries 7.x.2.3  
Font Awesome 7.x.2.6  


