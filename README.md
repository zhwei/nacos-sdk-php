# nacos-sdk-php

A PHP implementation of Nacos OpenAPI.

see: https://nacos.io/zh-cn/docs/open-API.html

## Required

- PHP ^7.0

## Install

```bash
composer require zhwei/nacos-sdk-php
```

## Getting Started

```php
use Nacos\NacosClient;

$client = new NacosClient('localhost', 8848);

$dataId = 'abc';
$group = 'test-group';
$value = $client->getConfig($dataId, $group);
```
