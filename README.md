# Geohash
[![Build Status](https://travis-ci.org/Eleme/geohash.png?branch=master)](https://travis-ci.org/Eleme/geohash)

Simple php geohash class

### Install
You may install Geohash with Composer (recommended) or manually.

```json
require: {
    "geohash/geohash": "dev-master"
}
```

### Usage
Encode a coordinates:

```php
<?php
require "vendor/autoload.php";

use Geohash\Geohash;

echo Geohash::encode(31.283131, 121.500831); // wtw3uyfjqw61
```

Decode a geohash:

```php
<?php
require "vendor/autoload.php";

use Geohash\Geohash;

list($lat, $lng) = Geohash::decode('wtw3uyfjqw61');
echo $lat, ', ', $lng; // 31.283131, 121.500831
```
