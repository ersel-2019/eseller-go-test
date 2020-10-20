# ActivePairing

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PairingId** | Pointer to **string** |  | [optional] 
**DeviceInfo** | Pointer to [**DeviceInfo**](DeviceInfo.md) |  | [optional] 

## Methods

### NewActivePairing

`func NewActivePairing() *ActivePairing`

NewActivePairing instantiates a new ActivePairing object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewActivePairingWithDefaults

`func NewActivePairingWithDefaults() *ActivePairing`

NewActivePairingWithDefaults instantiates a new ActivePairing object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPairingId

`func (o *ActivePairing) GetPairingId() string`

GetPairingId returns the PairingId field if non-nil, zero value otherwise.

### GetPairingIdOk

`func (o *ActivePairing) GetPairingIdOk() (*string, bool)`

GetPairingIdOk returns a tuple with the PairingId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPairingId

`func (o *ActivePairing) SetPairingId(v string)`

SetPairingId sets PairingId field to given value.

### HasPairingId

`func (o *ActivePairing) HasPairingId() bool`

HasPairingId returns a boolean if a field has been set.

### GetDeviceInfo

`func (o *ActivePairing) GetDeviceInfo() DeviceInfo`

GetDeviceInfo returns the DeviceInfo field if non-nil, zero value otherwise.

### GetDeviceInfoOk

`func (o *ActivePairing) GetDeviceInfoOk() (*DeviceInfo, bool)`

GetDeviceInfoOk returns a tuple with the DeviceInfo field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeviceInfo

`func (o *ActivePairing) SetDeviceInfo(v DeviceInfo)`

SetDeviceInfo sets DeviceInfo field to given value.

### HasDeviceInfo

`func (o *ActivePairing) HasDeviceInfo() bool`

HasDeviceInfo returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


