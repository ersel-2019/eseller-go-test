# \PairingApi

All URIs are relative to *https://some.host.com/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ConfirmPairing**](PairingApi.md#ConfirmPairing) | **Put** /pair-confirm/{pairingId} | Confirmes the ongoing pairing. The request will block until either the onboard GW button is pressed or the request times out (30s)
[**DoublePhysicalButtonTap**](PairingApi.md#DoublePhysicalButtonTap) | **Post** /double-button-tap | Simulates pressing the physical button on the GW twice
[**GetGWStatus**](PairingApi.md#GetGWStatus) | **Get** /gw-status | Returns the status of the GW
[**InitPairing**](PairingApi.md#InitPairing) | **Post** /pair-init | Initiates the pairing flow.
[**SinglePhysicalButtonTap**](PairingApi.md#SinglePhysicalButtonTap) | **Post** /single-button-tap | Simulates pressing the physical button on the GW once



## ConfirmPairing

> AccessInfo ConfirmPairing(ctx, pairingId).Execute()

Confirmes the ongoing pairing. The request will block until either the onboard GW button is pressed or the request times out (30s)

### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {
    pairingId := "pairingId_example" // string | Identifier for the active pairing

    configuration := openapiclient.NewConfiguration()
    api_client := openapiclient.NewAPIClient(configuration)
    resp, r, err := api_client.PairingApi.ConfirmPairing(context.Background(), pairingId).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `PairingApi.ConfirmPairing``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `ConfirmPairing`: AccessInfo
    fmt.Fprintf(os.Stdout, "Response from `PairingApi.ConfirmPairing`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**pairingId** | **string** | Identifier for the active pairing | 

### Other Parameters

Other parameters are passed through a pointer to a apiConfirmPairingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**AccessInfo**](AccessInfo.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DoublePhysicalButtonTap

> DoublePhysicalButtonTap(ctx).Execute()

Simulates pressing the physical button on the GW twice

### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {

    configuration := openapiclient.NewConfiguration()
    api_client := openapiclient.NewAPIClient(configuration)
    resp, r, err := api_client.PairingApi.DoublePhysicalButtonTap(context.Background()).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `PairingApi.DoublePhysicalButtonTap``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiDoublePhysicalButtonTapRequest struct via the builder pattern


### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetGWStatus

> GWStatus GetGWStatus(ctx).Execute()

Returns the status of the GW

### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {

    configuration := openapiclient.NewConfiguration()
    api_client := openapiclient.NewAPIClient(configuration)
    resp, r, err := api_client.PairingApi.GetGWStatus(context.Background()).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `PairingApi.GetGWStatus``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetGWStatus`: GWStatus
    fmt.Fprintf(os.Stdout, "Response from `PairingApi.GetGWStatus`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetGWStatusRequest struct via the builder pattern


### Return type

[**GWStatus**](GWStatus.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## InitPairing

> PairingInfo InitPairing(ctx).DeviceInfo(deviceInfo).Execute()

Initiates the pairing flow.

### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {
    deviceInfo := *openapiclient.NewDeviceInfo("Nickname_example") // DeviceInfo | Client supplies a nickname and device info (optional)

    configuration := openapiclient.NewConfiguration()
    api_client := openapiclient.NewAPIClient(configuration)
    resp, r, err := api_client.PairingApi.InitPairing(context.Background()).DeviceInfo(deviceInfo).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `PairingApi.InitPairing``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `InitPairing`: PairingInfo
    fmt.Fprintf(os.Stdout, "Response from `PairingApi.InitPairing`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiInitPairingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **deviceInfo** | [**DeviceInfo**](DeviceInfo.md) | Client supplies a nickname and device info | 

### Return type

[**PairingInfo**](PairingInfo.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SinglePhysicalButtonTap

> SinglePhysicalButtonTap(ctx).Execute()

Simulates pressing the physical button on the GW once

### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {

    configuration := openapiclient.NewConfiguration()
    api_client := openapiclient.NewAPIClient(configuration)
    resp, r, err := api_client.PairingApi.SinglePhysicalButtonTap(context.Background()).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `PairingApi.SinglePhysicalButtonTap``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiSinglePhysicalButtonTapRequest struct via the builder pattern


### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

