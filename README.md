"# drup8task" 
"Tasks Completed

Task 1
created a drup8task module called custom.
* Implemented hook_form_FORM-ID_alter, This function will Add a New field in Site information page
* Site Api key value stores in /drup8task/drup8task/config/install/drup8task.settings.yml file

Task 2
created a new menu as /nodecheck/{key}/{nid} to return json object
* created a controller to match siteapikey and nodeid , 
* if Key doesn't match it will respond access denied 
* if key matches but node id is wrong, it will respond as 'not a node'
* if key and node both matches, it will respond json object 

Conclusion
Refered drupal.org and stackoverflow.com
spended 2 hours to complete these tasks
Background Information
When logged in as the administrator, the "Site Information" form can be found at the path /admin/config/system/site-information.

Requirements
This module needs to alter the existing Drupal "Site Information" form. Specifics:

A new form text field named "Site API Key" needs to be added to the "Site Information" form with the default value of “No API Key yet”.
When this form is submitted, the value that the user entered for this field should be saved as the system variable named "siteapikey".
A Drupal message should inform the user that the Site API Key has been saved with that value.
When this form is visited after the "Site API Key" is saved, the field should be populated with the correct value.
The text of the "Save configuration" button should change to "Update Configuration".
This module also provides a URL that responds with a JSON representation of a given node with the content type "page" only if the previously submitted API Key and a node id (nid) of an appropriate node are present, otherwise it will respond with "access denied"."
