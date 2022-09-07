## Verify it works without the eloquent driver
run composer install

create an .env and configure it according to your setup 

Navigate to {app_url}/api/collections/news/entries
and verfiy that you se some data

## Steps to reproduce the error

1. run composer require statamic/eloquent-driver
2. run php artisan migrate
3. run php please eloquent:import-assets &&
php please eloquent:import-blueprints &&
php please eloquent:import-collections &&
php please eloquent:import-entries &&
php please eloquent:import-forms &&
php please eloquent:import-globals &&
php please eloquent:import-navs &&
php please eloquent:import-revisions &&
php please eloquent:import-taxonomies

1. Then navigate to {app_url}/api/collections/news/entries 
and you will encounter an error
