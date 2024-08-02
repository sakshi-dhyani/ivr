# SpControllerApi

All URIs are relative to *http://62.72.57.205:8098*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**addSpPositionDataUsingPOST**](SpControllerApi.md#addSpPositionDataUsingPOST) | **POST** /addSpPositionData | addSpPositionData |
| [**downloadfileUsingGET**](SpControllerApi.md#downloadfileUsingGET) | **GET** /downloadfile/{fileName} | downloadfile |
| [**getUsersUsingGET**](SpControllerApi.md#getUsersUsingGET) | **GET** /getUsers/{spId} | getUsers |
| [**logoutUsingGET**](SpControllerApi.md#logoutUsingGET) | **GET** /logout/{spId} | logout |
| [**resetPasswordUsingPOST**](SpControllerApi.md#resetPasswordUsingPOST) | **POST** /resetPassword | resetPassword |
| [**signinUsingPOST1**](SpControllerApi.md#signinUsingPOST1) | **POST** /signin | signin |


<a id="addSpPositionDataUsingPOST"></a>
# **addSpPositionDataUsingPOST**
> Response addSpPositionDataUsingPOST(spId, position, text, type)

addSpPositionData

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.SpControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    SpControllerApi apiInstance = new SpControllerApi(defaultClient);
    String spId = "spId_example"; // String | spId
    String position = "position_example"; // String | position
    String text = "text_example"; // String | text
    String type = "type_example"; // String | type
    try {
      Response result = apiInstance.addSpPositionDataUsingPOST(spId, position, text, type);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling SpControllerApi#addSpPositionDataUsingPOST");
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
| **spId** | **String**| spId | |
| **position** | **String**| position | [optional] |
| **text** | **String**| text | [optional] |
| **type** | **String**| type | [optional] |

### Return type

[**Response**](Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **201** | Created |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not Found |  -  |

<a id="downloadfileUsingGET"></a>
# **downloadfileUsingGET**
> Resource downloadfileUsingGET(fileName)

downloadfile

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.SpControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    SpControllerApi apiInstance = new SpControllerApi(defaultClient);
    String fileName = "fileName_example"; // String | fileName
    try {
      Resource result = apiInstance.downloadfileUsingGET(fileName);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling SpControllerApi#downloadfileUsingGET");
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
| **fileName** | **String**| fileName | |

### Return type

[**Resource**](Resource.md)

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

<a id="getUsersUsingGET"></a>
# **getUsersUsingGET**
> Response getUsersUsingGET(spId)

getUsers

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.SpControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    SpControllerApi apiInstance = new SpControllerApi(defaultClient);
    Integer spId = 56; // Integer | spId
    try {
      Response result = apiInstance.getUsersUsingGET(spId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling SpControllerApi#getUsersUsingGET");
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

<a id="logoutUsingGET"></a>
# **logoutUsingGET**
> Response logoutUsingGET(spId)

logout

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.SpControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    SpControllerApi apiInstance = new SpControllerApi(defaultClient);
    Integer spId = 56; // Integer | spId
    try {
      Response result = apiInstance.logoutUsingGET(spId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling SpControllerApi#logoutUsingGET");
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

<a id="resetPasswordUsingPOST"></a>
# **resetPasswordUsingPOST**
> Response resetPasswordUsingPOST(serviceProvider)

resetPassword

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.SpControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    SpControllerApi apiInstance = new SpControllerApi(defaultClient);
    ServiceProvider serviceProvider = new ServiceProvider(); // ServiceProvider | serviceProvider
    try {
      Response result = apiInstance.resetPasswordUsingPOST(serviceProvider);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling SpControllerApi#resetPasswordUsingPOST");
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
| **serviceProvider** | [**ServiceProvider**](ServiceProvider.md)| serviceProvider | |

### Return type

[**Response**](Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |
| **201** | Created |  -  |
| **401** | Unauthorized |  -  |
| **403** | Forbidden |  -  |
| **404** | Not Found |  -  |

<a id="signinUsingPOST1"></a>
# **signinUsingPOST1**
> SigninResponse signinUsingPOST1(email, password)

signin

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.SpControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    SpControllerApi apiInstance = new SpControllerApi(defaultClient);
    String email = "email_example"; // String | email
    String password = "password_example"; // String | password
    try {
      SigninResponse result = apiInstance.signinUsingPOST1(email, password);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling SpControllerApi#signinUsingPOST1");
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

