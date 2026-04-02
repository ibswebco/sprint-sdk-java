# ModelloApi

All URIs are relative to *https://api.sprintco.it/v2*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**v2modelliDestroy**](ModelloApi.md#v2modelliDestroy) | **DELETE** /modelli/{modello} | Remove the specified resource from storage |
| [**v2modelliIndex**](ModelloApi.md#v2modelliIndex) | **GET** /modelli | Display a listing of the resource |
| [**v2modelliShow**](ModelloApi.md#v2modelliShow) | **GET** /modelli/{modello} | Display the specified resource |
| [**v2modelliStore**](ModelloApi.md#v2modelliStore) | **POST** /modelli | Store a newly created resource in storage |
| [**v2modelliUpdate**](ModelloApi.md#v2modelliUpdate) | **PUT** /modelli/{modello} | Update the specified resource in storage |


<a id="v2modelliDestroy"></a>
# **v2modelliDestroy**
> v2modelliDestroy(modello)

Remove the specified resource from storage

### Example
```java
// Import classes:
import it.ibswebco.sprint.ApiClient;
import it.ibswebco.sprint.ApiException;
import it.ibswebco.sprint.Configuration;
import it.ibswebco.sprint.auth.*;
import it.ibswebco.sprint.models.*;
import it.ibswebco.sprint.ModelloApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://api.sprintco.it/v2");
    
    // Configure HTTP bearer authorization: http
    HttpBearerAuth http = (HttpBearerAuth) defaultClient.getAuthentication("http");
    http.setBearerToken("BEARER TOKEN");

    ModelloApi apiInstance = new ModelloApi(defaultClient);
    Integer modello = 56; // Integer | The modello idm1
    try {
      apiInstance.v2modelliDestroy(modello);
    } catch (ApiException e) {
      System.err.println("Exception when calling ModelloApi#v2modelliDestroy");
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
| **modello** | **Integer**| The modello idm1 | |

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
| **204** | No content |  -  |
| **403** | Authorization error |  -  |
| **404** | Not found |  -  |
| **401** | Unauthenticated |  -  |

<a id="v2modelliIndex"></a>
# **v2modelliIndex**
> Object v2modelliIndex()

Display a listing of the resource

### Example
```java
// Import classes:
import it.ibswebco.sprint.ApiClient;
import it.ibswebco.sprint.ApiException;
import it.ibswebco.sprint.Configuration;
import it.ibswebco.sprint.auth.*;
import it.ibswebco.sprint.models.*;
import it.ibswebco.sprint.ModelloApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://api.sprintco.it/v2");
    
    // Configure HTTP bearer authorization: http
    HttpBearerAuth http = (HttpBearerAuth) defaultClient.getAuthentication("http");
    http.setBearerToken("BEARER TOKEN");

    ModelloApi apiInstance = new ModelloApi(defaultClient);
    try {
      Object result = apiInstance.v2modelliIndex();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling ModelloApi#v2modelliIndex");
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

<a id="v2modelliShow"></a>
# **v2modelliShow**
> Object v2modelliShow(modello)

Display the specified resource

### Example
```java
// Import classes:
import it.ibswebco.sprint.ApiClient;
import it.ibswebco.sprint.ApiException;
import it.ibswebco.sprint.Configuration;
import it.ibswebco.sprint.auth.*;
import it.ibswebco.sprint.models.*;
import it.ibswebco.sprint.ModelloApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://api.sprintco.it/v2");
    
    // Configure HTTP bearer authorization: http
    HttpBearerAuth http = (HttpBearerAuth) defaultClient.getAuthentication("http");
    http.setBearerToken("BEARER TOKEN");

    ModelloApi apiInstance = new ModelloApi(defaultClient);
    Integer modello = 56; // Integer | The modello idm1
    try {
      Object result = apiInstance.v2modelliShow(modello);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling ModelloApi#v2modelliShow");
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
| **modello** | **Integer**| The modello idm1 | |

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

<a id="v2modelliStore"></a>
# **v2modelliStore**
> Object v2modelliStore(v2modelliStoreRequest)

Store a newly created resource in storage

### Example
```java
// Import classes:
import it.ibswebco.sprint.ApiClient;
import it.ibswebco.sprint.ApiException;
import it.ibswebco.sprint.Configuration;
import it.ibswebco.sprint.auth.*;
import it.ibswebco.sprint.models.*;
import it.ibswebco.sprint.ModelloApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://api.sprintco.it/v2");
    
    // Configure HTTP bearer authorization: http
    HttpBearerAuth http = (HttpBearerAuth) defaultClient.getAuthentication("http");
    http.setBearerToken("BEARER TOKEN");

    ModelloApi apiInstance = new ModelloApi(defaultClient);
    V2modelliStoreRequest v2modelliStoreRequest = new V2modelliStoreRequest(); // V2modelliStoreRequest | 
    try {
      Object result = apiInstance.v2modelliStore(v2modelliStoreRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling ModelloApi#v2modelliStore");
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
| **v2modelliStoreRequest** | [**V2modelliStoreRequest**](V2modelliStoreRequest.md)|  | |

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

<a id="v2modelliUpdate"></a>
# **v2modelliUpdate**
> Object v2modelliUpdate(modello, v2modelliUpdateRequest)

Update the specified resource in storage

### Example
```java
// Import classes:
import it.ibswebco.sprint.ApiClient;
import it.ibswebco.sprint.ApiException;
import it.ibswebco.sprint.Configuration;
import it.ibswebco.sprint.auth.*;
import it.ibswebco.sprint.models.*;
import it.ibswebco.sprint.ModelloApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://api.sprintco.it/v2");
    
    // Configure HTTP bearer authorization: http
    HttpBearerAuth http = (HttpBearerAuth) defaultClient.getAuthentication("http");
    http.setBearerToken("BEARER TOKEN");

    ModelloApi apiInstance = new ModelloApi(defaultClient);
    Integer modello = 56; // Integer | The modello idm1
    V2modelliUpdateRequest v2modelliUpdateRequest = new V2modelliUpdateRequest(); // V2modelliUpdateRequest | 
    try {
      Object result = apiInstance.v2modelliUpdate(modello, v2modelliUpdateRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling ModelloApi#v2modelliUpdate");
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
| **modello** | **Integer**| The modello idm1 | |
| **v2modelliUpdateRequest** | [**V2modelliUpdateRequest**](V2modelliUpdateRequest.md)|  | |

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

