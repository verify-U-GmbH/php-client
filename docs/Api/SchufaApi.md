# OpenAPI\Client\SchufaApi

All URIs are relative to *https://app.verify-u.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createSchufaById**](SchufaApi.md#createSchufaById) | **POST** /schufa | schufa/{id}



## createSchufaById

> \OpenAPI\Client\Model\InlineResponse2002 createSchufaById($body)

schufa/{id}

Creates a Schufa call for a client.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new OpenAPI\Client\Api\SchufaApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\Body1(); // Body1 | Address data

try {
    $result = $apiInstance->createSchufaById($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SchufaApi->createSchufaById: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Body1**](../Model/.md)| Address data |

### Return type

[**\OpenAPI\Client\Model\InlineResponse2002**](../Model/InlineResponse2002.md)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../../README.md#documentation-for-models)
[[Back to README]](../../README.md)

