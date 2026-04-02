# VistoApi

All URIs are relative to *https://api.sprintco.it/v2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**v2vistiDestroy**](VistoApi.md#v2vistiDestroy) | **DELETE** /visti/{visto} | Remove the specified resource from storage |
| [**v2vistiIndex**](VistoApi.md#v2vistiIndex) | **GET** /visti | Display a listing of the resource |
| [**v2vistiShow**](VistoApi.md#v2vistiShow) | **GET** /visti/{visto} | Display the specified resource |
| [**v2vistiStore**](VistoApi.md#v2vistiStore) | **POST** /visti | Store a newly created resource in storage |
| [**v2vistiUpdate**](VistoApi.md#v2vistiUpdate) | **PUT** /visti/{visto} | Update the specified resource in storage |


<a id="v2vistiDestroy"></a>
# **v2vistiDestroy**
> v2vistiDestroy(visto)

Remove the specified resource from storage

### Example
```java
// Import classes:
import it.ibswebco.spint.ApiClient;
import it.ibswebco.spint.ApiException;
import it.ibswebco.spint.Configuration;
import it.ibswebco.spint.auth.*;
import it.ibswebco.spint.models.*;
import it.ibswebco.sprint.VistoApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://api.sprintco.it/v2");
    
    // Configure HTTP bearer authorization: http
    HttpBearerAuth http = (HttpBearerAuth) defaultClient.getAuthentication("http");
    http.setBearerToken("BEARER TOKEN");

    VistoApi apiInstance = new VistoApi(defaultClient);
    String visto = "visto_example"; // String | The visto cod
    try {
      apiInstance.v2vistiDestroy(visto);
    } catch (ApiException e) {
      System.err.println("Exception when calling VistoApi#v2vistiDestroy");
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
| **visto** | **String**| The visto cod | |

### Return type

null (empty response body)

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

<a id="v2vistiIndex"></a>
# **v2vistiIndex**
> Object v2vistiIndex()

Display a listing of the resource

### Example
```java
// Import classes:
import it.ibswebco.spint.ApiClient;
import it.ibswebco.spint.ApiException;
import it.ibswebco.spint.Configuration;
import it.ibswebco.spint.auth.*;
import it.ibswebco.spint.models.*;
import it.ibswebco.sprint.VistoApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://api.sprintco.it/v2");
    
    // Configure HTTP bearer authorization: http
    HttpBearerAuth http = (HttpBearerAuth) defaultClient.getAuthentication("http");
    http.setBearerToken("BEARER TOKEN");

    VistoApi apiInstance = new VistoApi(defaultClient);
    try {
      Object result = apiInstance.v2vistiIndex();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling VistoApi#v2vistiIndex");
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

<a id="v2vistiShow"></a>
# **v2vistiShow**
> Object v2vistiShow(visto)

Display the specified resource

### Example
```java
// Import classes:
import it.ibswebco.spint.ApiClient;
import it.ibswebco.spint.ApiException;
import it.ibswebco.spint.Configuration;
import it.ibswebco.spint.auth.*;
import it.ibswebco.spint.models.*;
import it.ibswebco.sprint.VistoApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://api.sprintco.it/v2");
    
    // Configure HTTP bearer authorization: http
    HttpBearerAuth http = (HttpBearerAuth) defaultClient.getAuthentication("http");
    http.setBearerToken("BEARER TOKEN");

    VistoApi apiInstance = new VistoApi(defaultClient);
    String visto = "visto_example"; // String | The visto cod
    try {
      Object result = apiInstance.v2vistiShow(visto);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling VistoApi#v2vistiShow");
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
| **visto** | **String**| The visto cod | |

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

<a id="v2vistiStore"></a>
# **v2vistiStore**
> Object v2vistiStore(v2vistiStoreRequest)

Store a newly created resource in storage

### Example
```java
// Import classes:
import it.ibswebco.spint.ApiClient;
import it.ibswebco.spint.ApiException;
import it.ibswebco.spint.Configuration;
import it.ibswebco.spint.auth.*;
import it.ibswebco.spint.models.*;
import it.ibswebco.sprint.VistoApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://api.sprintco.it/v2");
    
    // Configure HTTP bearer authorization: http
    HttpBearerAuth http = (HttpBearerAuth) defaultClient.getAuthentication("http");
    http.setBearerToken("BEARER TOKEN");

    VistoApi apiInstance = new VistoApi(defaultClient);
    V2vistiStoreRequest v2vistiStoreRequest = new V2vistiStoreRequest(); // V2vistiStoreRequest | 
    try {
      Object result = apiInstance.v2vistiStore(v2vistiStoreRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling VistoApi#v2vistiStore");
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
| **v2vistiStoreRequest** | [**V2vistiStoreRequest**](V2vistiStoreRequest.md)|  | |

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

<a id="v2vistiUpdate"></a>
# **v2vistiUpdate**
> Object v2vistiUpdate(visto, v2vistiUpdateRequest)

Update the specified resource in storage

### Example
```java
// Import classes:
import it.ibswebco.spint.ApiClient;
import it.ibswebco.spint.ApiException;
import it.ibswebco.spint.Configuration;
import it.ibswebco.spint.auth.*;
import it.ibswebco.spint.models.*;
import it.ibswebco.sprint.VistoApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://api.sprintco.it/v2");
    
    // Configure HTTP bearer authorization: http
    HttpBearerAuth http = (HttpBearerAuth) defaultClient.getAuthentication("http");
    http.setBearerToken("BEARER TOKEN");

    VistoApi apiInstance = new VistoApi(defaultClient);
    String visto = "visto_example"; // String | The visto cod
    V2vistiUpdateRequest v2vistiUpdateRequest = new V2vistiUpdateRequest(); // V2vistiUpdateRequest | 
    try {
      Object result = apiInstance.v2vistiUpdate(visto, v2vistiUpdateRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling VistoApi#v2vistiUpdate");
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
| **visto** | **String**| The visto cod | |
| **v2vistiUpdateRequest** | [**V2vistiUpdateRequest**](V2vistiUpdateRequest.md)|  | |

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

