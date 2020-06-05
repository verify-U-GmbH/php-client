# OpenAPI\Client\IdentificationsApi

All URIs are relative to *https://verify-u.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getIdentificationById**](IdentificationsApi.md#getIdentificationById) | **GET** /identifications/{id} | identifications/{id}
[**getIdentificationDocumentById**](IdentificationsApi.md#getIdentificationDocumentById) | **GET** /identifications/id-document/{id} | identifications/id-document/{id}
[**getIdentificationsList**](IdentificationsApi.md#getIdentificationsList) | **GET** /identifications | identifications



## getIdentificationById

> \OpenAPI\Client\Model\InlineResponse2001 getIdentificationById($id)

identifications/{id}

Returns details of identification. Supply the unique identifier of the identification, received in OAuth response to the redirect URL

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new OpenAPI\Client\Api\IdentificationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the requested identification

try {
    $result = $apiInstance->getIdentificationById($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling IdentificationsApi->getIdentificationById: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**string**](../Model/.md)| ID of the requested identification |

### Return type

[**\OpenAPI\Client\Model\InlineResponse2001**](../Model/InlineResponse2001.md)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../../README.md#documentation-for-models)
[[Back to README]](../../README.md)


## getIdentificationDocumentById

> \SplFileObject getIdentificationDocumentById($id)

identifications/id-document/{id}

Returns id-document file uploaded during identification

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new OpenAPI\Client\Api\IdentificationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the id-document

try {
    $result = $apiInstance->getIdentificationDocumentById($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling IdentificationsApi->getIdentificationDocumentById: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**string**](../Model/.md)| ID of the id-document |

### Return type

[**\SplFileObject**](../Model/\SplFileObject.md)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: image/jpeg, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../../README.md#documentation-for-models)
[[Back to README]](../../README.md)


## getIdentificationsList

> \OpenAPI\Client\Model\InlineResponse200[] getIdentificationsList()

identifications

Returns the last 10 identifications as a list

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new OpenAPI\Client\Api\IdentificationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getIdentificationsList();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling IdentificationsApi->getIdentificationsList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\OpenAPI\Client\Model\InlineResponse200[]**](../Model/InlineResponse200.md)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../../README.md#documentation-for-models)
[[Back to README]](../../README.md)

