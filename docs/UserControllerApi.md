# UserControllerApi

All URIs are relative to *http://62.72.57.205:8098*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**editProfileUsingPUT**](UserControllerApi.md#editProfileUsingPUT) | **PUT** /user/editProfile | editProfile |
| [**signinUsingPOST2**](UserControllerApi.md#signinUsingPOST2) | **POST** /user/signin | signin |


<a id="editProfileUsingPUT"></a>
# **editProfileUsingPUT**
> Response editProfileUsingPUT(name, spId, userId)

editProfile

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.UserControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    UserControllerApi apiInstance = new UserControllerApi(defaultClient);
    String name = "name_example"; // String | name
    String spId = "spId_example"; // String | spId
    String userId = "userId_example"; // String | userId
    try {
      Response result = apiInstance.editProfileUsingPUT(name, spId, userId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserControllerApi#editProfileUsingPUT");
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
| **name** | **String**| name | [optional] |
| **spId** | **String**| spId | [optional] |
| **userId** | **String**| userId | [optional] |

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

<a id="signinUsingPOST2"></a>
# **signinUsingPOST2**
> SigninResponse signinUsingPOST2(phoneNumber, spId)

signin

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.UserControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    UserControllerApi apiInstance = new UserControllerApi(defaultClient);
    String phoneNumber = "phoneNumber_example"; // String | phoneNumber
    String spId = "spId_example"; // String | spId
    try {
      SigninResponse result = apiInstance.signinUsingPOST2(phoneNumber, spId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling UserControllerApi#signinUsingPOST2");
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
| **phoneNumber** | **String**| phoneNumber | [optional] |
| **spId** | **String**| spId | [optional] |

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

