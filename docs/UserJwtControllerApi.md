# UserJwtControllerApi

All URIs are relative to *https://localhost:7080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**authorizeUsingPOST**](UserJwtControllerApi.md#authorizeUsingPOST) | **POST** /api/authenticate | authorize


<a name="authorizeUsingPOST"></a>
# **authorizeUsingPOST**
> ResponseEntity authorizeUsingPOST(loginVM)

authorize

authorize

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.UserJwtControllerApi;


UserJwtControllerApi apiInstance = new UserJwtControllerApi();
LoginVM loginVM = new LoginVM(); // LoginVM | loginVM
try {
    ResponseEntity result = apiInstance.authorizeUsingPOST(loginVM);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserJwtControllerApi#authorizeUsingPOST");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **loginVM** | [**LoginVM**](LoginVM.md)| loginVM |

### Return type

[**ResponseEntity**](ResponseEntity.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

