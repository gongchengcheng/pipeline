# \DeploymentApi

All URIs are relative to *http://localhost:9090*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeleteDeployment**](DeploymentApi.md#DeleteDeployment) | **Delete** /api/v1/orgs/{orgId}/clusters/{id}/deployments/{name} | Delete deployment
[**GetDeployment**](DeploymentApi.md#GetDeployment) | **Get** /api/v1/orgs/{orgId}/clusters/{id}/deployments/{name} | Get deployment details
[**HelmDeploymentStatus**](DeploymentApi.md#HelmDeploymentStatus) | **Head** /api/v1/orgs/{orgId}/clusters/{id}/deployments/{name} | Check deployment status
[**UpdateDeployment**](DeploymentApi.md#UpdateDeployment) | **Put** /api/v1/orgs/{orgId}/clusters/{id}/deployments/{name} | Update deployment


# **DeleteDeployment**
> DeleteDeploymentResponse DeleteDeployment(ctx, orgId, id, name)
Delete deployment

Deleting a Helm deployment

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **orgId** | **int32**| Organization identification | 
  **id** | **int32**| Selected cluster identification (number) | 
  **name** | **string**| Deployment name | 

### Return type

[**DeleteDeploymentResponse**](DeleteDeploymentResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **GetDeployment**
> GetDeploymentResponse GetDeployment(ctx, orgId, id, name)
Get deployment details

Retrieves the details of a deployment

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **orgId** | **int32**| Organization identification | 
  **id** | **int32**| Selected cluster identification (number) | 
  **name** | **string**| Deployment name | 

### Return type

[**GetDeploymentResponse**](GetDeploymentResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **HelmDeploymentStatus**
> HelmDeploymentStatus(ctx, orgId, id, name)
Check deployment status

Checking the status of a deployment through the Helm client API

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **orgId** | **int32**| Organization identification | 
  **id** | **int32**| Selected cluster identification (number) | 
  **name** | **string**| Deployment name | 

### Return type

 (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **UpdateDeployment**
> CreateUpdateDeploymentResponse UpdateDeployment(ctx, orgId, id, name, createUpdateDeploymentRequest)
Update deployment

Updating a Helm deployment

### Required Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
  **orgId** | **int32**| Organization identification | 
  **id** | **int32**| Selected cluster identification (number) | 
  **name** | **string**| Deployment name | 
  **createUpdateDeploymentRequest** | [**CreateUpdateDeploymentRequest**](CreateUpdateDeploymentRequest.md)|  | 

### Return type

[**CreateUpdateDeploymentResponse**](CreateUpdateDeploymentResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

