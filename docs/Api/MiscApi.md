# NGP\MiscApi

All URIs are relative to *https://api.securevan.com/v4*

Method | HTTP request | Description
------------- | ------------- | -------------
[**echoesPost**](MiscApi.md#echoesPost) | **POST** /echoes | Hello world
[**events4306Get**](MiscApi.md#events4306Get) | **GET** /events/4306 | Get event details
[**people100879417CanvassResponsesPost**](MiscApi.md#people100879417CanvassResponsesPost) | **POST** /people/100879417/canvassResponses | Collect canvass data
[**peopleFindOrCreatePost**](MiscApi.md#peopleFindOrCreatePost) | **POST** /people/findOrCreate | Create a volunteer record
[**signupsPost**](MiscApi.md#signupsPost) | **POST** /signups | RSVP to an event


# **echoesPost**
> echoesPost($content_type, $body)

Hello world



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure HTTP basic authorization: auth
$config = NGP\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new NGP\Api\MiscApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$content_type = "content_type_example"; // string | 
$body = new \NGP\Model\HelloworldRequest(); // \NGP\Model\HelloworldRequest | 

try {
    $apiInstance->echoesPost($content_type, $body);
} catch (Exception $e) {
    echo 'Exception when calling MiscApi->echoesPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **string**|  |
 **body** | [**\NGP\Model\HelloworldRequest**](../Model/HelloworldRequest.md)|  |

### Return type

void (empty response body)

### Authorization

[auth](../../README.md#auth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **events4306Get**
> events4306Get($expand, $authorization)

Get event details



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure HTTP basic authorization: auth
$config = NGP\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new NGP\Api\MiscApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$expand = "expand_example"; // string | 
$authorization = "authorization_example"; // string | 

try {
    $apiInstance->events4306Get($expand, $authorization);
} catch (Exception $e) {
    echo 'Exception when calling MiscApi->events4306Get: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **expand** | **string**|  |
 **authorization** | **string**|  |

### Return type

void (empty response body)

### Authorization

[auth](../../README.md#auth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **people100879417CanvassResponsesPost**
> people100879417CanvassResponsesPost($content_type, $authorization, $body)

Collect canvass data



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure HTTP basic authorization: auth
$config = NGP\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new NGP\Api\MiscApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$content_type = "content_type_example"; // string | 
$authorization = "authorization_example"; // string | 
$body = new \NGP\Model\CollectcanvassdataRequest(); // \NGP\Model\CollectcanvassdataRequest | 

try {
    $apiInstance->people100879417CanvassResponsesPost($content_type, $authorization, $body);
} catch (Exception $e) {
    echo 'Exception when calling MiscApi->people100879417CanvassResponsesPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **string**|  |
 **authorization** | **string**|  |
 **body** | [**\NGP\Model\CollectcanvassdataRequest**](../Model/CollectcanvassdataRequest.md)|  |

### Return type

void (empty response body)

### Authorization

[auth](../../README.md#auth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **peopleFindOrCreatePost**
> peopleFindOrCreatePost($content_type, $authorization, $body)

Create a volunteer record



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure HTTP basic authorization: auth
$config = NGP\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new NGP\Api\MiscApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$content_type = "content_type_example"; // string | 
$authorization = "authorization_example"; // string | 
$body = new \NGP\Model\CreateavolunteerrecordRequest(); // \NGP\Model\CreateavolunteerrecordRequest | 

try {
    $apiInstance->peopleFindOrCreatePost($content_type, $authorization, $body);
} catch (Exception $e) {
    echo 'Exception when calling MiscApi->peopleFindOrCreatePost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **string**|  |
 **authorization** | **string**|  |
 **body** | [**\NGP\Model\CreateavolunteerrecordRequest**](../Model/CreateavolunteerrecordRequest.md)|  |

### Return type

void (empty response body)

### Authorization

[auth](../../README.md#auth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **signupsPost**
> signupsPost($content_type, $authorization, $body)

RSVP to an event



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure HTTP basic authorization: auth
$config = NGP\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new NGP\Api\MiscApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$content_type = "content_type_example"; // string | 
$authorization = "authorization_example"; // string | 
$body = new \NGP\Model\RSVPtoaneventRequest(); // \NGP\Model\RSVPtoaneventRequest | 

try {
    $apiInstance->signupsPost($content_type, $authorization, $body);
} catch (Exception $e) {
    echo 'Exception when calling MiscApi->signupsPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **string**|  |
 **authorization** | **string**|  |
 **body** | [**\NGP\Model\RSVPtoaneventRequest**](../Model/RSVPtoaneventRequest.md)|  |

### Return type

void (empty response body)

### Authorization

[auth](../../README.md#auth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

