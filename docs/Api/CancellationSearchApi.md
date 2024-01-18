# macropage\SDKs\ebay\rest\postorder\CancellationSearchApi

All URIs are relative to https://api.ebay.com/post-order/v2, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**searchCancellations()**](CancellationSearchApi.md#searchCancellations) | **GET** /cancellation/search | Search for order cancellations |


## `searchCancellations()`

```php
searchCancellations($cancelId, $creationDateRangeFrom, $creationDateRangeTo, $itemId, $legacyOrderId, $limit, $offset, $role, $sort, $transactionId): \macropage\SDKs\ebay\rest\postorder\Model\FindCancelResponse
```

Search for order cancellations

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new macropage\SDKs\ebay\rest\postorder\Api\CancellationSearchApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$cancelId = 'cancelId_example'; // string
$creationDateRangeFrom = 'creationDateRangeFrom_example'; // string
$creationDateRangeTo = 'creationDateRangeTo_example'; // string
$itemId = 'itemId_example'; // string
$legacyOrderId = 'legacyOrderId_example'; // string
$limit = 'limit_example'; // string
$offset = 'offset_example'; // string
$role = 'role_example'; // string
$sort = 'sort_example'; // string
$transactionId = 'transactionId_example'; // string

try {
    $result = $apiInstance->searchCancellations($cancelId, $creationDateRangeFrom, $creationDateRangeTo, $itemId, $legacyOrderId, $limit, $offset, $role, $sort, $transactionId);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CancellationSearchApi->searchCancellations: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cancelId** | **string**|  | [optional] |
| **creationDateRangeFrom** | **string**|  | [optional] |
| **creationDateRangeTo** | **string**|  | [optional] |
| **itemId** | **string**|  | [optional] |
| **legacyOrderId** | **string**|  | [optional] |
| **limit** | **string**|  | [optional] |
| **offset** | **string**|  | [optional] |
| **role** | **string**|  | [optional] |
| **sort** | **string**|  | [optional] |
| **transactionId** | **string**|  | [optional] |

### Return type

[**\macropage\SDKs\ebay\rest\postorder\Model\FindCancelResponse**](../Model/FindCancelResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
