<<<<<<< HEAD
Php client library for Insightly web API (v2.1)
===============================================

The Insightly PHP SDK enables PHP developers to quickly integrate their applications with the Insightly REST API (version 2.1).

NOTE: this SDK currently only works with version 2.1 of the Insightly API. To use version 2.2, you'll need to modify this library, or you can use Swagger (www.swagger.io) to auto-generate an SDK (it can generate SDKs for over a dozen different target languages).

NOTE: works best with PHP version 5.5.x, some users have reported issues with parse errors using older versions of PHP.

The library handles low level communication, authentication,
and encoding to minimize learning curve and debugging overhead for new users.
The library provides the ability to read/write/delete
all major Insightly objects, including:

* Contacts
* Events
* Organizations
* Opportunities
* Projects

To use the library, simply add insightly.php to your PHP include-path.
Then making requests is as simple as:

```php
require("insightly.php");

$i = new Insightly('your-api-key');
$contacts = $i->getContacts();
```

The API interface is provided by the `Insightly` class.
Please refer to the source-code documentation for more information.

The library was authored by Nathan Davis, and is currently in beta.
=======
# PHP-Insightly
## Getting started
### Composer
`composer require ggdx/php-insightly`


### Example:
```php
$insightly = new Insightly($api_key, $api_version) // $api_version is optional, v2.2 is default
$insightly->getContacts();
```

Documentation will follow but for now, all methods are fully documented in the code.

For $data arrays, please see [Insightly API Docs](https://api.insight.ly/v2.2/) for requirements. For the most part, Insightly is pretty flexible with "required" data but there are certain situations where a minimum dataset is required.

For the Laravel 5 service provider, look [here](https://github.com/ggdx/LaravelInsightly)
>>>>>>> php-insightly/master
