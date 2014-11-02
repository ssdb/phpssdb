phpssdb
=======

SSDB PHP Client

For More Details, See: [Official PHP Client Document](http://ssdb.io/docs/zh_cn/php/)

## Installation

PHP 5.3+ is required. There is no need for additional libraries.

Append dependency into composer.json

```
	...
	"require": {
		...
		"ssdb/phpssdb": "dev-master"
	}
	...
```

## Basic Using

```php
<?php

$ssdb = new SSDB\Client('127.0.0.1', 8888);

var_dump($ssdb->set('test', time()));

echo $ssdb->get('test') . "\n";

var_dump($ssdb->del('test'));

var_dump($ssdb->get('test'));

```

