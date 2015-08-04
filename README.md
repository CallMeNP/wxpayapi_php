# wxpayapi_php
【微信支付】API对应的SDK和调用示例。微信官方代码。仅为自动加载和配置文件做修改。

# 使用
## require
composer require即可。参见 https://packagist.org/packages/callmenp/wxpayapi_php

## 配置
然后在laravel框架的config/services.php 中添加相关配置：
```php
	'wxpay' => [
		'appid'=>'wx426b3015555a46be',
		'mchid'=>'1225312702',
		'key'=>'e10adc3949ba59abbe56e057f20f883e',
		'appsecret'=>'01c6d59a3f9024db6336662ac95c8e74',
		'sslcert_path'=>'../cert/apiclient_cert.pem',
		'sslkey_path'=>'../cert/apiclient_key.pem',
		'curl_proxy_host'=>'0.0.0.0',
		'curl_proxy_port'=>0,
		'report_levenl'=>1,
	],
```

## 使用
相关类都声明在根命名空间下。

```php
$wxpay=new \WxPayApi();
```
