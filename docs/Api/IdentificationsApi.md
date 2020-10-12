# OpenAPI\Client\IdentificationsApi

All URIs are relative to *https://app.verify-u.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getAuditDocumentById**](IdentificationsApi.md#getAuditDocumentById) | **GET** /identifications/audit-document/{document_id} | identifications/audit-document/{document_id}
[**getEsignById**](IdentificationsApi.md#getEsignById) | **GET** /identifications/esign/{id} | identifications/e-sign/{id}
[**getIdentificationById**](IdentificationsApi.md#getIdentificationById) | **GET** /identifications/{id} | identifications/{id}
[**getIdentificationDocumentById**](IdentificationsApi.md#getIdentificationDocumentById) | **GET** /identifications/id-document/{document_id} | identifications/id-document/{document_id}
[**getIdentificationVideoById**](IdentificationsApi.md#getIdentificationVideoById) | **GET** /identifications/video/{id} | identifications/video/{id}
[**getIdentificationsList**](IdentificationsApi.md#getIdentificationsList) | **GET** /identifications | identifications
[**getSchufaById**](IdentificationsApi.md#getSchufaById) | **GET** /identifications/schufa/{id} | identifications/schufa/{id}



## getAuditDocumentById

> \SplFileObject getAuditDocumentById($document_id)

identifications/audit-document/{document_id}

Returns the client's audit document image created during identification.

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
$document_id = 'document_id_example'; // string | ID of the audit-document

try {
    $result = $apiInstance->getAuditDocumentById($document_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling IdentificationsApi->getAuditDocumentById: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | [**string**](../Model/.md)| ID of the audit-document |

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


## getEsignById

> \SplFileObject getEsignById($id)

identifications/e-sign/{id}

Returns the client's contract document, signed by the customer with digital signature.

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
$id = 'id_example'; // string | ID of the identification

try {
    $result = $apiInstance->getEsignById($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling IdentificationsApi->getEsignById: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**string**](../Model/.md)| ID of the identification |

### Return type

[**\SplFileObject**](../Model/\SplFileObject.md)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/pdf, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../../README.md#documentation-for-models)
[[Back to README]](../../README.md)


## getIdentificationById

> \OpenAPI\Client\Model\InlineResponse200 getIdentificationById($id)

identifications/{id}

Returns details of a single identification.

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

[**\OpenAPI\Client\Model\InlineResponse200**](../Model/InlineResponse200.md)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../../README.md#documentation-for-models)
[[Back to README]](../../README.md)


## getIdentificationDocumentById

> \SplFileObject getIdentificationDocumentById($document_id)

identifications/id-document/{document_id}

Returns the client's id document image used for identification.

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
$document_id = 'document_id_example'; // string | ID of the id-document

try {
    $result = $apiInstance->getIdentificationDocumentById($document_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling IdentificationsApi->getIdentificationDocumentById: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **document_id** | [**string**](../Model/.md)| ID of the id-document |

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


## getIdentificationVideoById

> \SplFileObject getIdentificationVideoById($id)

identifications/video/{id}

Returns the client's liveness video recording used for identification.

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
$id = 'id_example'; // string | ID of the identification

try {
    $result = $apiInstance->getIdentificationVideoById($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling IdentificationsApi->getIdentificationVideoById: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**string**](../Model/.md)| ID of the identification |

### Return type

[**\SplFileObject**](../Model/\SplFileObject.md)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: video/mp4, application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../../README.md#documentation-for-models)
[[Back to README]](../../README.md)


## getIdentificationsList

> \OpenAPI\Client\Model\InlineResponse200[] getIdentificationsList($limit, $offset, $status)

identifications

Returns the latest identifications as a list. Most recent identifications appear first. Customize your query with the following parameters.

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
$limit = 56; // int | Limits the number of identifications to be returned. Limit can range between 1 and 100, and the default is 10.
$offset = 56; // int | Specifies the page number of the identifications to be returned. Default is 0.
$status = 'status_example'; // string | When set, only identifications of this status are returned. Default is `init`.   * `init` - Identification has been initially started   * `id_verified` - Id document check completed   * `f2f_verified` - Face-to-face check completed   * `face_detected` - Face check completed   * `liveness_detected` - Liveness check completed   * `schufa_ident_verified` - Schufa ident check completed   * `schufa_bank_verified` - Schufa bank check completed   * `esign_verified` - E-sign document signed   * `complete` - Identification has been completed successfully

try {
    $result = $apiInstance->getIdentificationsList($limit, $offset, $status);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling IdentificationsApi->getIdentificationsList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**| Limits the number of identifications to be returned. Limit can range between 1 and 100, and the default is 10. | [optional]
 **offset** | **int**| Specifies the page number of the identifications to be returned. Default is 0. | [optional]
 **status** | **string**| When set, only identifications of this status are returned. Default is &#x60;init&#x60;.   * &#x60;init&#x60; - Identification has been initially started   * &#x60;id_verified&#x60; - Id document check completed   * &#x60;f2f_verified&#x60; - Face-to-face check completed   * &#x60;face_detected&#x60; - Face check completed   * &#x60;liveness_detected&#x60; - Liveness check completed   * &#x60;schufa_ident_verified&#x60; - Schufa ident check completed   * &#x60;schufa_bank_verified&#x60; - Schufa bank check completed   * &#x60;esign_verified&#x60; - E-sign document signed   * &#x60;complete&#x60; - Identification has been completed successfully | [optional]

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


## getSchufaById

> \OpenAPI\Client\Model\InlineResponse2001 getSchufaById($id)

identifications/schufa/{id}

Returns the client's Schufa result.

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
$id = 'id_example'; // string | ID of the identification

try {
    $result = $apiInstance->getSchufaById($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling IdentificationsApi->getSchufaById: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | [**string**](../Model/.md)| ID of the identification |

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

