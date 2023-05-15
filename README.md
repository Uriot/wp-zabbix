# wp-zabbix
Zabbix client for WordPress by [Sven Wappler](https://wappler.systems)

Install composer by Elliot Urizar

## What does it do?

This plugin provides a REST API endpoint for the [Zabbix](https://www.zabbix.com/) monitoring system.

## Installation

  1. Install the wp-zabbix plugin.
  2. Define a key in your _wp-config.php_ file. For example:
     
     `define('WPZABBIX_KEY', 'eoij4r93440frexampler0rugt0rug0tru');`

     Please use a long key for best security.

  3. Import the zabbix template from wp-zabbix/template/wordpress.xml
  4. Create a host in zabbix
  5. Add a macro to this host called:
     `{$WORDPRESS_CLIENT_KEY}` with the value of your generated key
     
## Composer Installation to WordPress-bedrock


1. Add to Composer.json
```
"require": {
        ...,
        ...,
        "uriot/wp-zabbix": "dev-master"
    },
    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/Uriot/wp-zabbix.git"
        }
    ],
```
and in the path of your project 

`composer update`
