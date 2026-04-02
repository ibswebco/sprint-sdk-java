# RichiestaApi

All URIs are relative to *https://api.sprintco.it/v2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**v2richiesteDestroy**](RichiestaApi.md#v2richiesteDestroy) | **DELETE** /richieste/{richiesta} | Remove the specified resource from storage |
| [**v2richiesteIndex**](RichiestaApi.md#v2richiesteIndex) | **GET** /richieste | Display a listing of the resource |
| [**v2richiesteShow**](RichiestaApi.md#v2richiesteShow) | **GET** /richieste/{richiesta} | Display the specified resource |
| [**v2richiesteStore**](RichiestaApi.md#v2richiesteStore) | **POST** /richieste | Store a newly created resource in storage |
| [**v2richiesteUpdate**](RichiestaApi.md#v2richiesteUpdate) | **PUT** /richieste/{richiesta} | Update the specified resource in storage |


<a id="v2richiesteDestroy"></a>
# **v2richiesteDestroy**
> Object v2richiesteDestroy(richiesta)

Remove the specified resource from storage

### Example
```java
// Import classes:
import it.ibswebco.sprint.ApiClient;
import it.ibswebco.sprint.ApiException;
import it.ibswebco.sprint.Configuration;
import it.ibswebco.sprint.auth.*;
import it.ibswebco.sprint.models.*;
import it.ibswebco.sprint.RichiestaApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://api.sprintco.it/v2");
    
    // Configure HTTP bearer authorization: http
    HttpBearerAuth http = (HttpBearerAuth) defaultClient.getAuthentication("http");
    http.setBearerToken("BEARER TOKEN");

    RichiestaApi apiInstance = new RichiestaApi(defaultClient);
    String richiesta = "richiesta_example"; // String | The richiesta r1 codric
    try {
      Object result = apiInstance.v2richiesteDestroy(richiesta);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RichiestaApi#v2richiesteDestroy");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **richiesta** | **String**| The richiesta r1 codric | |

### Return type

**Object**

### Authorization

[http](../README.md#http)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |
| **403** | Authorization error |  -  |
| **404** | Not found |  -  |
| **401** | Unauthenticated |  -  |

<a id="v2richiesteIndex"></a>
# **v2richiesteIndex**
> Object v2richiesteIndex()

Display a listing of the resource

### Example
```java
// Import classes:
import it.ibswebco.sprint.ApiClient;
import it.ibswebco.sprint.ApiException;
import it.ibswebco.sprint.Configuration;
import it.ibswebco.sprint.auth.*;
import it.ibswebco.sprint.models.*;
import it.ibswebco.sprint.RichiestaApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://api.sprintco.it/v2");
    
    // Configure HTTP bearer authorization: http
    HttpBearerAuth http = (HttpBearerAuth) defaultClient.getAuthentication("http");
    http.setBearerToken("BEARER TOKEN");

    RichiestaApi apiInstance = new RichiestaApi(defaultClient);
    try {
      Object result = apiInstance.v2richiesteIndex();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RichiestaApi#v2richiesteIndex");
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

**Object**

### Authorization

[http](../README.md#http)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |
| **401** | Unauthenticated |  -  |

<a id="v2richiesteShow"></a>
# **v2richiesteShow**
> Object v2richiesteShow(richiesta)

Display the specified resource

### Example
```java
// Import classes:
import it.ibswebco.sprint.ApiClient;
import it.ibswebco.sprint.ApiException;
import it.ibswebco.sprint.Configuration;
import it.ibswebco.sprint.auth.*;
import it.ibswebco.sprint.models.*;
import it.ibswebco.sprint.RichiestaApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://api.sprintco.it/v2");
    
    // Configure HTTP bearer authorization: http
    HttpBearerAuth http = (HttpBearerAuth) defaultClient.getAuthentication("http");
    http.setBearerToken("BEARER TOKEN");

    RichiestaApi apiInstance = new RichiestaApi(defaultClient);
    String richiesta = "richiesta_example"; // String | The richiesta r1 codric
    try {
      Object result = apiInstance.v2richiesteShow(richiesta);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RichiestaApi#v2richiesteShow");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **richiesta** | **String**| The richiesta r1 codric | |

### Return type

**Object**

### Authorization

[http](../README.md#http)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |
| **403** | Authorization error |  -  |
| **404** | Not found |  -  |
| **401** | Unauthenticated |  -  |

<a id="v2richiesteStore"></a>
# **v2richiesteStore**
> Object v2richiesteStore(v2richiesteStoreRequest)

Store a newly created resource in storage

### Example
```java
// Import classes:
import it.ibswebco.sprint.ApiClient;
import it.ibswebco.sprint.ApiException;
import it.ibswebco.sprint.Configuration;
import it.ibswebco.sprint.auth.*;
import it.ibswebco.sprint.models.*;
import it.ibswebco.sprint.RichiestaApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://api.sprintco.it/v2");
    
    // Configure HTTP bearer authorization: http
    HttpBearerAuth http = (HttpBearerAuth) defaultClient.getAuthentication("http");
    http.setBearerToken("BEARER TOKEN");

    RichiestaApi apiInstance = new RichiestaApi(defaultClient);
    V2richiesteStoreRequest v2richiesteStoreRequest = new V2richiesteStoreRequest(); // V2richiesteStoreRequest | 
    try {
      Object result = apiInstance.v2richiesteStore(v2richiesteStoreRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RichiestaApi#v2richiesteStore");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **v2richiesteStoreRequest** | [**V2richiesteStoreRequest**](V2richiesteStoreRequest.md)|  | |

### Return type

**Object**

### Authorization

[http](../README.md#http)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |
| **403** | Authorization error |  -  |
| **422** | Validation error |  -  |
| **401** | Unauthenticated |  -  |

<a id="v2richiesteUpdate"></a>
# **v2richiesteUpdate**
> Object v2richiesteUpdate(richiesta, v2richiesteUpdateRequest)

Update the specified resource in storage

### Example
```java
// Import classes:
import it.ibswebco.sprint.ApiClient;
import it.ibswebco.sprint.ApiException;
import it.ibswebco.sprint.Configuration;
import it.ibswebco.sprint.auth.*;
import it.ibswebco.sprint.models.*;
import it.ibswebco.sprint.RichiestaApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://api.sprintco.it/v2");
    
    // Configure HTTP bearer authorization: http
    HttpBearerAuth http = (HttpBearerAuth) defaultClient.getAuthentication("http");
    http.setBearerToken("BEARER TOKEN");

    RichiestaApi apiInstance = new RichiestaApi(defaultClient);
    String richiesta = "richiesta_example"; // String | The richiesta r1 codric
    V2richiesteUpdateRequest v2richiesteUpdateRequest = new V2richiesteUpdateRequest(); // V2richiesteUpdateRequest | 
    try {
      Object result = apiInstance.v2richiesteUpdate(richiesta, v2richiesteUpdateRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling RichiestaApi#v2richiesteUpdate");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **richiesta** | **String**| The richiesta r1 codric | |
| **v2richiesteUpdateRequest** | [**V2richiesteUpdateRequest**](V2richiesteUpdateRequest.md)|  | |

### Return type

**Object**

### Authorization

[http](../README.md#http)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** |  |  -  |
| **403** | Authorization error |  -  |
| **422** | Validation error |  -  |
| **404** | Not found |  -  |
| **401** | Unauthenticated |  -  |

