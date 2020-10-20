# DeviceInfo

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Nickname** | **string** |  | 
**Vendor** | Pointer to **string** |  | [optional] 
**Model** | Pointer to **string** |  | [optional] 
**OsVersion** | Pointer to **string** |  | [optional] 
**IpAddress** | Pointer to **string** |  | [optional] 

## Methods

### NewDeviceInfo

`func NewDeviceInfo(nickname string, ) *DeviceInfo`

NewDeviceInfo instantiates a new DeviceInfo object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDeviceInfoWithDefaults

`func NewDeviceInfoWithDefaults() *DeviceInfo`

NewDeviceInfoWithDefaults instantiates a new DeviceInfo object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetNickname

`func (o *DeviceInfo) GetNickname() string`

GetNickname returns the Nickname field if non-nil, zero value otherwise.

### GetNicknameOk

`func (o *DeviceInfo) GetNicknameOk() (*string, bool)`

GetNicknameOk returns a tuple with the Nickname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNickname

`func (o *DeviceInfo) SetNickname(v string)`

SetNickname sets Nickname field to given value.


### GetVendor

`func (o *DeviceInfo) GetVendor() string`

GetVendor returns the Vendor field if non-nil, zero value otherwise.

### GetVendorOk

`func (o *DeviceInfo) GetVendorOk() (*string, bool)`

GetVendorOk returns a tuple with the Vendor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVendor

`func (o *DeviceInfo) SetVendor(v string)`

SetVendor sets Vendor field to given value.

### HasVendor

`func (o *DeviceInfo) HasVendor() bool`

HasVendor returns a boolean if a field has been set.

### GetModel

`func (o *DeviceInfo) GetModel() string`

GetModel returns the Model field if non-nil, zero value otherwise.

### GetModelOk

`func (o *DeviceInfo) GetModelOk() (*string, bool)`

GetModelOk returns a tuple with the Model field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModel

`func (o *DeviceInfo) SetModel(v string)`

SetModel sets Model field to given value.

### HasModel

`func (o *DeviceInfo) HasModel() bool`

HasModel returns a boolean if a field has been set.

### GetOsVersion

`func (o *DeviceInfo) GetOsVersion() string`

GetOsVersion returns the OsVersion field if non-nil, zero value otherwise.

### GetOsVersionOk

`func (o *DeviceInfo) GetOsVersionOk() (*string, bool)`

GetOsVersionOk returns a tuple with the OsVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOsVersion

`func (o *DeviceInfo) SetOsVersion(v string)`

SetOsVersion sets OsVersion field to given value.

### HasOsVersion

`func (o *DeviceInfo) HasOsVersion() bool`

HasOsVersion returns a boolean if a field has been set.

### GetIpAddress

`func (o *DeviceInfo) GetIpAddress() string`

GetIpAddress returns the IpAddress field if non-nil, zero value otherwise.

### GetIpAddressOk

`func (o *DeviceInfo) GetIpAddressOk() (*string, bool)`

GetIpAddressOk returns a tuple with the IpAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIpAddress

`func (o *DeviceInfo) SetIpAddress(v string)`

SetIpAddress sets IpAddress field to given value.

### HasIpAddress

`func (o *DeviceInfo) HasIpAddress() bool`

HasIpAddress returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


