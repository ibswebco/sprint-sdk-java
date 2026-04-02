# DefaultApi

All URIs are relative to *https://api.sprintco.it/v2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**v2**](DefaultApi.md#v2) | **GET** /test |  |


<a id="v2"></a>
# **v2**
> V2200Response v2()



### Example
```java
// Import classes:
import it.ibswebco.spint.ApiClient;
import it.ibswebco.spint.ApiException;
import it.ibswebco.spint.Configuration;
import it.ibswebco.spint.auth.*;
import it.ibswebco.spint.models.*;
import it.ibswebco.sprint.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://api.sprintco.it/v2");
    
    // Configure HTTP bearer authorization: http
    HttpBearerAuth http = (HttpBearerAuth) defaultClient.getAuthentication("http");
    http.setBearerToken("BEARER TOKEN");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    try {
      V2200Response result = apiInstance.v2();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#v2");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**V2200Response**](V2200Response.md)

### Authorization

[http](../README.md#http)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |

