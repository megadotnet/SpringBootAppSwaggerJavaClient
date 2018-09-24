# UserAccountControllerApi

All URIs are relative to *https://localhost:7080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**activateAccountUsingGET**](UserAccountControllerApi.md#activateAccountUsingGET) | **GET** /api/activate | activateAccount
[**changePasswordUsingPOST**](UserAccountControllerApi.md#changePasswordUsingPOST) | **POST** /api/account/change_password | changePassword
[**finishPasswordResetUsingPOST**](UserAccountControllerApi.md#finishPasswordResetUsingPOST) | **POST** /api/account/reset_password/finish | finishPasswordReset
[**getAccountUsingGET**](UserAccountControllerApi.md#getAccountUsingGET) | **GET** /api/account | getAccount
[**isAuthenticatedUsingGET**](UserAccountControllerApi.md#isAuthenticatedUsingGET) | **GET** /api/authenticate | isAuthenticated
[**registerAccountUsingPOST**](UserAccountControllerApi.md#registerAccountUsingPOST) | **POST** /api/register | registerAccount
[**requestPasswordResetUsingPOST**](UserAccountControllerApi.md#requestPasswordResetUsingPOST) | **POST** /api/account/reset_password/init | requestPasswordReset
[**saveAccountUsingPOST**](UserAccountControllerApi.md#saveAccountUsingPOST) | **POST** /api/account | saveAccount


<a name="activateAccountUsingGET"></a>
# **activateAccountUsingGET**
> String activateAccountUsingGET(key)

activateAccount

activate Account

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.UserAccountControllerApi;


UserAccountControllerApi apiInstance = new UserAccountControllerApi();
String key = "key_example"; // String | key
try {
    String result = apiInstance.activateAccountUsingGET(key);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserAccountControllerApi#activateAccountUsingGET");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key** | **String**| key |

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a name="changePasswordUsingPOST"></a>
# **changePasswordUsingPOST**
> ResponseEntity changePasswordUsingPOST(password)

changePassword

change Password

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.UserAccountControllerApi;


UserAccountControllerApi apiInstance = new UserAccountControllerApi();
String password = "password_example"; // String | password
try {
    ResponseEntity result = apiInstance.changePasswordUsingPOST(password);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserAccountControllerApi#changePasswordUsingPOST");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **password** | **String**| password |

### Return type

[**ResponseEntity**](ResponseEntity.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: text/plain

<a name="finishPasswordResetUsingPOST"></a>
# **finishPasswordResetUsingPOST**
> String finishPasswordResetUsingPOST(keyAndPassword)

finishPasswordReset

finish PasswordReset

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.UserAccountControllerApi;


UserAccountControllerApi apiInstance = new UserAccountControllerApi();
KeyAndPasswordVM keyAndPassword = new KeyAndPasswordVM(); // KeyAndPasswordVM | keyAndPassword
try {
    String result = apiInstance.finishPasswordResetUsingPOST(keyAndPassword);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserAccountControllerApi#finishPasswordResetUsingPOST");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **keyAndPassword** | [**KeyAndPasswordVM**](KeyAndPasswordVM.md)| keyAndPassword |

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: text/plain

<a name="getAccountUsingGET"></a>
# **getAccountUsingGET**
> UserDTO getAccountUsingGET()

getAccount

get Account

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.UserAccountControllerApi;


UserAccountControllerApi apiInstance = new UserAccountControllerApi();
try {
    UserDTO result = apiInstance.getAccountUsingGET();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserAccountControllerApi#getAccountUsingGET");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**UserDTO**](UserDTO.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a name="isAuthenticatedUsingGET"></a>
# **isAuthenticatedUsingGET**
> String isAuthenticatedUsingGET()

isAuthenticated

is Authenticated

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.UserAccountControllerApi;


UserAccountControllerApi apiInstance = new UserAccountControllerApi();
try {
    String result = apiInstance.isAuthenticatedUsingGET();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserAccountControllerApi#isAuthenticatedUsingGET");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a name="registerAccountUsingPOST"></a>
# **registerAccountUsingPOST**
> ResponseEntity registerAccountUsingPOST(managedUserVM)

registerAccount

register Account

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.UserAccountControllerApi;


UserAccountControllerApi apiInstance = new UserAccountControllerApi();
ManagedUserVM managedUserVM = new ManagedUserVM(); // ManagedUserVM | managedUserVM
try {
    ResponseEntity result = apiInstance.registerAccountUsingPOST(managedUserVM);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserAccountControllerApi#registerAccountUsingPOST");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **managedUserVM** | [**ManagedUserVM**](ManagedUserVM.md)| managedUserVM |

### Return type

[**ResponseEntity**](ResponseEntity.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json, text/plain

<a name="requestPasswordResetUsingPOST"></a>
# **requestPasswordResetUsingPOST**
> ResponseEntity requestPasswordResetUsingPOST(mail)

requestPasswordReset

request PasswordReset

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.UserAccountControllerApi;


UserAccountControllerApi apiInstance = new UserAccountControllerApi();
String mail = "mail_example"; // String | mail
try {
    ResponseEntity result = apiInstance.requestPasswordResetUsingPOST(mail);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserAccountControllerApi#requestPasswordResetUsingPOST");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mail** | **String**| mail |

### Return type

[**ResponseEntity**](ResponseEntity.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: text/plain

<a name="saveAccountUsingPOST"></a>
# **saveAccountUsingPOST**
> ResponseEntity saveAccountUsingPOST(userDTO)

saveAccount

save Account

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.UserAccountControllerApi;


UserAccountControllerApi apiInstance = new UserAccountControllerApi();
UserDTO userDTO = new UserDTO(); // UserDTO | userDTO
try {
    ResponseEntity result = apiInstance.saveAccountUsingPOST(userDTO);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserAccountControllerApi#saveAccountUsingPOST");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userDTO** | [**UserDTO**](UserDTO.md)| userDTO |

### Return type

[**ResponseEntity**](ResponseEntity.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

