
# Utils for WordPress

## What motivates me to create?
For every WordPress project, I have used repeatedly the same Utilities. So I have decided to make this repo for WP Community. 

## What you will get by using this?**
Reduce your extra codes from your actual project, write optimized code, prefix keys and lots more

## Requirements
Create a config file in your plugin root 
```php
/your-plugin-name/dynamic-utils.config.php
```


Return array with minimum these items. 
```php
return [
	'project_key' => 'content_restriction',
	'key_prefix'  => '_',
	'key_suffix'  => '_',
];
```


If you pass more items, and can access them using HeyMehedi\Utils\Config::get('your_key'), here is an example from real-project
```php
return [
	'version'     => '2.0.0',
	'min_php'     => '7.4',
	'db_version'  => '1.0.0',
	'menu_slug'   => 'all-in-one-content-restriction',
	'menu_cap'    => 'manage_options',
	'environment' => 'development',

	'project_key' => 'content_restriction',
	'key_prefix'  => '_',
	'key_suffix'  => '_',
];
```