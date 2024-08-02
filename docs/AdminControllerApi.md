# AdminControllerApi

All URIs are relative to *http://62.72.57.205:8098*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createServiceProviderUsingPOST**](AdminControllerApi.md#createServiceProviderUsingPOST) | **POST** /createServiceProvider | createServiceProvider |
| [**getAllServiceProvidersUsingGET**](AdminControllerApi.md#getAllServiceProvidersUsingGET) | **GET** /getAllServiceProviders | getAllServiceProviders |
| [**getAllUsersUsingGET**](AdminControllerApi.md#getAllUsersUsingGET) | **GET** /getAllUsers | getAllUsers |
| [**getSpPositionDataUsingGET**](AdminControllerApi.md#getSpPositionDataUsingGET) | **GET** /getSpPositionData/{spId} | getSpPositionData |
| [**getserviceProviderInfoUsingGET**](AdminControllerApi.md#getserviceProviderInfoUsingGET) | **GET** /getserviceProviderInfo/{uniqueId} | getserviceProviderInfo |
| [**signinUsingPOST**](AdminControllerApi.md#signinUsingPOST) | **POST** /admin/signin | signin |
| [**signupUsingPOST**](AdminControllerApi.md#signupUsingPOST) | **POST** /admin/signup | signup |


<a id="createServiceProviderUsingPOST"></a>
# **createServiceProviderUsingPOST**
> Response createServiceProviderUsingPOST(name, address, email, invokingNumbers)

createServiceProvider

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.AdminControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    AdminControllerApi apiInstance = new AdminControllerApi(defaultClient);
    String name = "name_example"; // String | name
    String address = "address_example"; // String | address
    String email = "email_example"; // String | email
    List<Integer> invokingNumbers = Arrays.asList(); // List<Integer> | invokingNumbers
    try {
      Response result = apiInstance.createServiceProviderUsingPOST(name, address, email, invokingNumbers);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminControllerApi#createServiceProviderUsingPOST");
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
| **name** | **String**| name | |
| **address** | **String**| address | [optional] |
| **email** | **String**| email | [optional] |
| **invokingNumbers** | [**List&lt;Integer&gt;**](Integer.md)| invokingNumbers | [optional] |

### Return type

[**Response**](Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **201** | Created |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not Found |  -  |

<a id="getAllServiceProvidersUsingGET"></a>
# **getAllServiceProvidersUsingGET**
> Response getAllServiceProvidersUsingGET()

getAllServiceProviders

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.AdminControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    AdminControllerApi apiInstance = new AdminControllerApi(defaultClient);
    try {
      Response result = apiInstance.getAllServiceProvidersUsingGET();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminControllerApi#getAllServiceProvidersUsingGET");
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

[**Response**](Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not Found |  -  |

<a id="getAllUsersUsingGET"></a>
# **getAllUsersUsingGET**
> Response getAllUsersUsingGET()

getAllUsers

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.AdminControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    AdminControllerApi apiInstance = new AdminControllerApi(defaultClient);
    try {
      Response result = apiInstance.getAllUsersUsingGET();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminControllerApi#getAllUsersUsingGET");
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

[**Response**](Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not Found |  -  |

<a id="getSpPositionDataUsingGET"></a>
# **getSpPositionDataUsingGET**
> Response getSpPositionDataUsingGET(spId)

getSpPositionData

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.AdminControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    AdminControllerApi apiInstance = new AdminControllerApi(defaultClient);
    Integer spId = 56; // Integer | spId
    try {
      Response result = apiInstance.getSpPositionDataUsingGET(spId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminControllerApi#getSpPositionDataUsingGET");
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
| **spId** | **Integer**| spId | |

### Return type

[**Response**](Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not Found |  -  |

<a id="getserviceProviderInfoUsingGET"></a>
# **getserviceProviderInfoUsingGET**
> Response getserviceProviderInfoUsingGET(uniqueId)

getserviceProviderInfo

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.AdminControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    AdminControllerApi apiInstance = new AdminControllerApi(defaultClient);
    String uniqueId = "uniqueId_example"; // String | uniqueId
    try {
      Response result = apiInstance.getserviceProviderInfoUsingGET(uniqueId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminControllerApi#getserviceProviderInfoUsingGET");
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
| **uniqueId** | **String**| uniqueId | |

### Return type

[**Response**](Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not Found |  -  |

<a id="signinUsingPOST"></a>
# **signinUsingPOST**
> SigninResponse signinUsingPOST(email, password)

signin

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.AdminControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    AdminControllerApi apiInstance = new AdminControllerApi(defaultClient);
    String email = "email_example"; // String | email
    String password = "password_example"; // String | password
    try {
      SigninResponse result = apiInstance.signinUsingPOST(email, password);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminControllerApi#signinUsingPOST");
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
| **email** | **String**| email | |
| **password** | **String**| password | [optional] |

### Return type

[**SigninResponse**](SigninResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **201** | Created |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not Found |  -  |

<a id="signupUsingPOST"></a>
# **signupUsingPOST**
> Response signupUsingPOST(email, name, password)

signup

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.AdminControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    AdminControllerApi apiInstance = new AdminControllerApi(defaultClient);
    String email = "email_example"; // String | email
    String name = "name_example"; // String | name
    String password = "password_example"; // String | password
    try {
      Response result = apiInstance.signupUsingPOST(email, name, password);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling AdminControllerApi#signupUsingPOST");
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
| **email** | **String**| email | |
| **name** | **String**| name | |
| **password** | **String**| password | [optional] |

### Return type

[**Response**](Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **201** | Created |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not Found |  -  |

