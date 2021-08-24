
# DDEV multisite setup for drupal

## Setup steps

- Clone the repo in your project root directory beside docroot or web foder.
- Run command ```cp .ddev/settings.ddev.php docroot/sites/default/settings.ddev.php``` .
- Import database using command for each site ``` ddev drush sql-sync @your_site_alias @self --uri=https://uk.ddev.site ```
- Please pass --uri=site_url with each command e.g ``` ddev drush cr --uri=https://uk.ddev.site ```  or cim ``` ddev drush cim --uri=https://uk.ddev.site ``` 

### Note: 
 - Make sure your your database name is same as hostname e.g for site(host name) uk database name is uk. Otherwise you would need to cutomise settings.ddev.php as per the change.

## References
- https://stackoverflow.com/questions/49785023/how-can-i-create-and-load-a-second-database-in-ddev 
