BacklogPHP
---

[Backlog API V2](http://developer.nulab-inc.com/ja/docs/backlog/api/2/) PHP Client.

# Setup

```sh
curl -sS https://getcomposer.org/installer | php
php composer.phar install
```

# How to use

```php
<?php
$backlog = new \Backlog\Client();
$backlog->setSpace($space)
    ->setApiKey($token);

// GET /api/v2/projects
$response = $backlog->projects->get();

var_dump($response->getBody());
```

[more sample](https://github.com/m-s-modified/BacklogPHP/blob/master/sample.php)

# Test

```sh
php composer.phar test
```

# CI Build Status

[![Build Status](https://travis-ci.org/m-s-modified/BacklogPHP.svg?branch=master)](https://travis-ci.org/m-s-modified/BacklogPHP)
