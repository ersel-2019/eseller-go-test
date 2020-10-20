# GWStatus

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**State** | Pointer to **string** |  | [optional] 
**LastSingleButtonTap** | Pointer to **string** |  | [optional] 
**LastDoubleButtonTap** | Pointer to **string** |  | [optional] 
**ActivePairing** | Pointer to [**ActivePairing**](ActivePairing.md) |  | [optional] 
**PairedDevices** | Pointer to [**[]DeviceInfo**](DeviceInfo.md) |  | [optional] 

## Methods

### NewGWStatus

`func NewGWStatus() *GWStatus`

NewGWStatus instantiates a new GWStatus object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGWStatusWithDefaults

`func NewGWStatusWithDefaults() *GWStatus`

NewGWStatusWithDefaults instantiates a new GWStatus object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetState

`func (o *GWStatus) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *GWStatus) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *GWStatus) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *GWStatus) HasState() bool`

HasState returns a boolean if a field has been set.

### GetLastSingleButtonTap

`func (o *GWStatus) GetLastSingleButtonTap() string`

GetLastSingleButtonTap returns the LastSingleButtonTap field if non-nil, zero value otherwise.

### GetLastSingleButtonTapOk

`func (o *GWStatus) GetLastSingleButtonTapOk() (*string, bool)`

GetLastSingleButtonTapOk returns a tuple with the LastSingleButtonTap field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSingleButtonTap

`func (o *GWStatus) SetLastSingleButtonTap(v string)`

SetLastSingleButtonTap sets LastSingleButtonTap field to given value.

### HasLastSingleButtonTap

`func (o *GWStatus) HasLastSingleButtonTap() bool`

HasLastSingleButtonTap returns a boolean if a field has been set.

### GetLastDoubleButtonTap

`func (o *GWStatus) GetLastDoubleButtonTap() string`

GetLastDoubleButtonTap returns the LastDoubleButtonTap field if non-nil, zero value otherwise.

### GetLastDoubleButtonTapOk

`func (o *GWStatus) GetLastDoubleButtonTapOk() (*string, bool)`

GetLastDoubleButtonTapOk returns a tuple with the LastDoubleButtonTap field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastDoubleButtonTap

`func (o *GWStatus) SetLastDoubleButtonTap(v string)`

SetLastDoubleButtonTap sets LastDoubleButtonTap field to given value.

### HasLastDoubleButtonTap

`func (o *GWStatus) HasLastDoubleButtonTap() bool`

HasLastDoubleButtonTap returns a boolean if a field has been set.

### GetActivePairing

`func (o *GWStatus) GetActivePairing() ActivePairing`

GetActivePairing returns the ActivePairing field if non-nil, zero value otherwise.

### GetActivePairingOk

`func (o *GWStatus) GetActivePairingOk() (*ActivePairing, bool)`

GetActivePairingOk returns a tuple with the ActivePairing field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActivePairing

`func (o *GWStatus) SetActivePairing(v ActivePairing)`

SetActivePairing sets ActivePairing field to given value.

### HasActivePairing

`func (o *GWStatus) HasActivePairing() bool`

HasActivePairing returns a boolean if a field has been set.

### GetPairedDevices

`func (o *GWStatus) GetPairedDevices() []DeviceInfo`

GetPairedDevices returns the PairedDevices field if non-nil, zero value otherwise.

### GetPairedDevicesOk

`func (o *GWStatus) GetPairedDevicesOk() (*[]DeviceInfo, bool)`

GetPairedDevicesOk returns a tuple with the PairedDevices field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPairedDevices

`func (o *GWStatus) SetPairedDevices(v []DeviceInfo)`

SetPairedDevices sets PairedDevices field to given value.

### HasPairedDevices

`func (o *GWStatus) HasPairedDevices() bool`

HasPairedDevices returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


