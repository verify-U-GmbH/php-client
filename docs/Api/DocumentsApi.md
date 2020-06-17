# OpenAPI\Client\DocumentsApi

All URIs are relative to *https://app.verify-u.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createDocument**](DocumentsApi.md#createDocument) | **POST** /documents | documents



## createDocument

> string createDocument($body)

documents

Transfers a contract document PDF to be signed by the client.   Store the returned `document_id` and append it to the identification request for the corresponding client.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure HTTP basic authorization: basicAuth
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new OpenAPI\Client\Api\DocumentsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \OpenAPI\Client\Model\Body(); // Body | Contract document pdf file

try {
    $result = $apiInstance->createDocument($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DocumentsApi->createDocument: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Body**](../Model/.md)| Contract document pdf file |

### Return type

**string**

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../../README.md#documentation-for-models)
[[Back to README]](../../README.md)

