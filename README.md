#Configuration/migration notes

##Views
Don't forget to update Drupal settings.php in order to pull in all custom fields

##Customizations
Confirm.tpl and ThankYou.tpl at  
sites/all/modules/civicrm/templates/CRM/Contribute/Form/Contribution

"contribution" => "membership registration"

(Will have to re-do with any code upgrade.)

###Style Extensions

/civicrm/admin/setting/url&reset=1

Add path to <waterwheel>/module/core/style/civicrm.css to the Custom CSS URL field. (This file is managed inside the waterwheel repository.)

##Drupal Modules: 

Views 7.x.3.13  
User Import 7.x.3.2  
Chaos 7.x.1.9  
Advanced Help 7.x.1.3  
Password Reset Landing Page 7.x.1.1  
Views Conditional 7.x.1.3
Menu Items Visibility 7.x.1.x-dev
