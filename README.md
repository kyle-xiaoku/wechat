# wechat
微信公众号、小程序简单，方便服务调用

## 关于
> - 此PHP SDK基于[腾讯官方API](https://developers.weixin.qq.com/doc/service/guide/)官方API构建。
> - 公众号、小程序接口调用。

## 运行环境
> - PHP 8.2及以上。

## 安装方法
### 通过 composer 安装
如果您通过composer管理您的项目依赖，可以在你的项目根目录运行：
```bash
$ composer require kyle/wechat
```
或者在你的`composer.json`中声明对wechat的依赖：
```php
"require": {
    "kyle/wechat": "*"
}
```
然后通过`composer install`安装依赖

## 快速使用
#### 获取公众号access_token
```php
<?php

use Kyle\Wechat\Wechat;

return Wechat::mp()->getAccessToken();
```