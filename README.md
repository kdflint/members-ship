#Configuration/migration notes

##Views
Don't forget to update Drupal settings.php in order to pull in all custom fields

Get the database mappings from CiviCRM here: http://northbridgetech.org/dev/members/index.php?q=civicrm/admin/setting/uf&reset=1

instructions: https://wiki.civicrm.org/confluence/display/CRMDOC41/Views3+Integration

##Code Customizations
Confirm.tpl and ThankYou.tpl at  
sites/all/modules/civicrm/templates/CRM/Contribute/Form/Contribution

"the contribution" => "your membership registration"

(Will have to re-do with any code upgrade.)

###Style Extensions

/civicrm/admin/setting/url&reset=1

Add path to <waterwheel>/module/core/style/civicrm.css to the Custom CSS URL field. (This file is managed inside the waterwheel repository.)

To: themes/bartik/css/style.css

Add at top: @import url("http://northbridgetech.org/apps/waterwheel/module/core/style/civicrm.css");

##Drupal Modules: 

Views 7.x.3.13  
User Import 7.x.3.2  
Chaos 7.x.1.9  
Advanced Help 7.x.1.3  
Password Reset Landing Page 7.x.1.1  
Views Conditional 7.x.1.3
Menu Items Visibility 7.x.1.x-dev
Token 7.x-1.6
