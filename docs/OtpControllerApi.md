# OtpControllerApi

All URIs are relative to *http://62.72.57.205:8098*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**generateOTPForResetPasswordUsingGET**](OtpControllerApi.md#generateOTPForResetPasswordUsingGET) | **GET** /sp/generateOTPForResetPassword/{email} | generateOTPForResetPassword |
| [**generateOTPForSignupUsingGET**](OtpControllerApi.md#generateOTPForSignupUsingGET) | **GET** /generateOTPForSignup/{email} | generateOTPForSignup |
| [**verifyOTPUsingPOST**](OtpControllerApi.md#verifyOTPUsingPOST) | **POST** /SP/verifyOTP | verifyOTP |


<a id="generateOTPForResetPasswordUsingGET"></a>
# **generateOTPForResetPasswordUsingGET**
> Response generateOTPForResetPasswordUsingGET(email)

generateOTPForResetPassword

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.OtpControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    OtpControllerApi apiInstance = new OtpControllerApi(defaultClient);
    String email = "email_example"; // String | email
    try {
      Response result = apiInstance.generateOTPForResetPasswordUsingGET(email);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling OtpControllerApi#generateOTPForResetPasswordUsingGET");
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

<a id="generateOTPForSignupUsingGET"></a>
# **generateOTPForSignupUsingGET**
> Response generateOTPForSignupUsingGET(email)

generateOTPForSignup

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.OtpControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    OtpControllerApi apiInstance = new OtpControllerApi(defaultClient);
    String email = "email_example"; // String | email
    try {
      Response result = apiInstance.generateOTPForSignupUsingGET(email);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling OtpControllerApi#generateOTPForSignupUsingGET");
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

<a id="verifyOTPUsingPOST"></a>
# **verifyOTPUsingPOST**
> Response verifyOTPUsingPOST(email, otp)

verifyOTP

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.OtpControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://62.72.57.205:8098");

    OtpControllerApi apiInstance = new OtpControllerApi(defaultClient);
    String email = "email_example"; // String | email
    String otp = "otp_example"; // String | otp
    try {
      Response result = apiInstance.verifyOTPUsingPOST(email, otp);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling OtpControllerApi#verifyOTPUsingPOST");
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
| **otp** | **String**| otp | |

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

