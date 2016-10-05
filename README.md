# ExpressionEngine 2 Config Files

Updates the default ExpressionEngine configuration files (`config.php` and `database.php`) to include more overrides and dynamically set variables for faster deployment and easier development. Intended to be simple and not involve adding any new files to the mix.

_(The idea behind creating an ExpressionEngine "master config" is not my own. Thanks to everyone who has openly shared their files.)_

Notes:

* Default ExpressionEngine configuration files were generated from version 2.11.3
* All configuration variables are not set to ExpressionEngine defaults. Some have been changed based on environment assumptions (listed below).

Assumptions:

* `index.php` will be removed from your URL.
* Templates will be saved as files.
* Strict URLs will be enabled
* 404 errors will use the `404/index` template_group/template.
* Template hit tracking should be turned off.
* Hidden template indicator should be a `.` instead of `_`.

Variables To Change Before Implementation:

* In `config.php`
  * `$config['license_contact']`
  * `$config['license_number']`
  * `$config['site_name']`
  * `$config['app_version']`
* In `database.php`
  * `$db['expressionengine']['hostname']`
  * `$db['expressionengine']['username']`
  * `$db['expressionengine']['password']`
  * `$db['expressionengine']['database']`
