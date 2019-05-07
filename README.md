# ![LOGO](logo.png) Cloud IoT **flow**ground Connector

## Description

A generated **flow**ground connector for the Cloud IoT API (version v1).

Generated from: https://api.apis.guru/v2/specs/googleapis.com/cloudiot/v1/swagger.json<br/>
Generated at: 2019-05-07T17:41:19+03:00

## API Description

Registers and manages IoT (Internet of Things) devices that connect to the Google Cloud Platform.


## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Deletes a device.

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - The name of the device. For example,
`projects/p0/locations/us-central1/registries/registry0/devices/device0` or
`projects/p0/locations/us-central1/registries/registry0/devices/{num_id}`.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Gets details about a device.

*Tags:* `projects`

#### Input Parameters
* `fieldMask` - _optional_ - The fields of the `Device` resource to be returned in the response. If the
field mask is unset or empty, all fields are returned.
* `name` - _required_ - The name of the device. For example,
`projects/p0/locations/us-central1/registries/registry0/devices/device0` or
`projects/p0/locations/us-central1/registries/registry0/devices/{num_id}`.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Updates a device.

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - The resource path name. For example,
`projects/p1/locations/us-central1/registries/registry0/devices/dev0` or
`projects/p1/locations/us-central1/registries/registry0/devices/{num_id}`.
When `name` is populated as a response from the service, it always ends
in the device numeric ID.
* `updateMask` - _optional_ - Only updates the `device` fields indicated by this mask.
The field mask must not be empty, and it must not contain fields that
are immutable or only set by the server.
Mutable top-level fields: `credentials`, `blocked`, and `metadata`
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists the last few versions of the device configuration in descending<br/>
> order (i.e.: newest first).

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - The name of the device. For example,
`projects/p0/locations/us-central1/registries/registry0/devices/device0` or
`projects/p0/locations/us-central1/registries/registry0/devices/{num_id}`.
* `numVersions` - _optional_ - The number of versions to list. Versions are listed in decreasing order of
the version number. The maximum number of versions retained is 10. If this
value is zero, it will return all the versions available.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists the last few versions of the device state in descending order (i.e.:<br/>
> newest first).

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - The name of the device. For example,
`projects/p0/locations/us-central1/registries/registry0/devices/device0` or
`projects/p0/locations/us-central1/registries/registry0/devices/{num_id}`.
* `numStates` - _optional_ - The number of states to list. States are listed in descending order of
update time. The maximum number of states retained is 10. If this
value is zero, it will return all the states available.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Modifies the configuration for the device, which is eventually sent from<br/>
> the Cloud IoT Core servers. Returns the modified configuration version and<br/>
> its metadata.

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - The name of the device. For example,
`projects/p0/locations/us-central1/registries/registry0/devices/device0` or
`projects/p0/locations/us-central1/registries/registry0/devices/{num_id}`.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Sends a command to the specified device. In order for a device to be able<br/>
> to receive commands, it must:<br/>
> 1) be connected to Cloud IoT Core using the MQTT protocol, and<br/>
> 2) be subscribed to the group of MQTT topics specified by<br/>
>    /devices/{device-id}/commands/#. This subscription will receive commands<br/>
>    at the top-level topic /devices/{device-id}/commands as well as commands<br/>
>    for subfolders, like /devices/{device-id}/commands/subfolder.<br/>
>    Note that subscribing to specific subfolders is not supported.<br/>
> If the command could not be delivered to the device, this method will<br/>
> return an error; in particular, if the device is not subscribed, this<br/>
> method will return FAILED_PRECONDITION. Otherwise, this method will<br/>
> return OK. If the subscription is QoS 1, at least once delivery will be<br/>
> guaranteed; for QoS 0, no acknowledgment will be expected from the device.

*Tags:* `projects`

#### Input Parameters
* `name` - _required_ - The name of the device. For example,
`projects/p0/locations/us-central1/registries/registry0/devices/device0` or
`projects/p0/locations/us-central1/registries/registry0/devices/{num_id}`.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### List devices in a device registry.

*Tags:* `projects`

#### Input Parameters
* `deviceIds` - _optional_ - A list of device string IDs. For example, `['device0', 'device12']`.
If empty, this field is ignored. Maximum IDs: 10,000
* `deviceNumIds` - _optional_ - A list of device numeric IDs. If empty, this field is ignored. Maximum
IDs: 10,000.
* `fieldMask` - _optional_ - The fields of the `Device` resource to be returned in the response. The
fields `id` and `num_id` are always returned, along with any
other fields specified.
* `gatewayListOptions.associationsDeviceId` - _optional_ - If set, returns only the gateways with which the specified device is
associated. The device ID can be numeric (`num_id`) or the user-defined
string (`id`). For example, if `456` is specified, returns only the
gateways to which the device with `num_id` 456 is bound.
* `gatewayListOptions.associationsGatewayId` - _optional_ - If set, only devices associated with the specified gateway are returned.
The gateway ID can be numeric (`num_id`) or the user-defined string
(`id`). For example, if `123` is specified, only devices bound to the
gateway with `num_id` 123 are returned.
* `gatewayListOptions.gatewayType` - _optional_ - If `GATEWAY` is specified, only gateways are returned. If `NON_GATEWAY`
is specified, only non-gateway devices are returned. If
`GATEWAY_TYPE_UNSPECIFIED` is specified, all devices are returned.
    Possible values: GATEWAY_TYPE_UNSPECIFIED, GATEWAY, NON_GATEWAY.
* `pageSize` - _optional_ - The maximum number of devices to return in the response. If this value
is zero, the service will select a default size. A call may return fewer
objects than requested. A non-empty `next_page_token` in the response
indicates that more data is available.
* `pageToken` - _optional_ - The value returned by the last `ListDevicesResponse`; indicates
that this is a continuation of a prior `ListDevices` call and
the system should return the next page of data.
* `parent` - _required_ - The device registry path. Required. For example,
`projects/my-project/locations/us-central1/registries/my-registry`.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Creates a device in a device registry.

*Tags:* `projects`

#### Input Parameters
* `parent` - _required_ - The name of the device registry where this device should be created.
For example,
`projects/example-project/locations/us-central1/registries/my-registry`.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Lists device registries.

*Tags:* `projects`

#### Input Parameters
* `pageSize` - _optional_ - The maximum number of registries to return in the response. If this value
is zero, the service will select a default size. A call may return fewer
objects than requested. A non-empty `next_page_token` in the response
indicates that more data is available.
* `pageToken` - _optional_ - The value returned by the last `ListDeviceRegistriesResponse`; indicates
that this is a continuation of a prior `ListDeviceRegistries` call and
the system should return the next page of data.
* `parent` - _required_ - The project and cloud region path. For example,
`projects/example-project/locations/us-central1`.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Creates a device registry that contains devices.

*Tags:* `projects`

#### Input Parameters
* `parent` - _required_ - The project and cloud region where this device registry must be created.
For example, `projects/example-project/locations/us-central1`.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Associates the device with the gateway.

*Tags:* `projects`

#### Input Parameters
* `parent` - _required_ - The name of the registry. For example,
`projects/example-project/locations/us-central1/registries/my-registry`.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Deletes the association between the device and the gateway.

*Tags:* `projects`

#### Input Parameters
* `parent` - _required_ - The name of the registry. For example,
`projects/example-project/locations/us-central1/registries/my-registry`.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Gets the access control policy for a resource.<br/>
> Returns an empty policy if the resource exists and does not have a policy<br/>
> set.

*Tags:* `projects`

#### Input Parameters
* `resource` - _required_ - REQUIRED: The resource for which the policy is being requested.
See the operation documentation for the appropriate value for this field.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Sets the access control policy on the specified resource. Replaces any<br/>
> existing policy.

*Tags:* `projects`

#### Input Parameters
* `resource` - _required_ - REQUIRED: The resource for which the policy is being specified.
See the operation documentation for the appropriate value for this field.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

### Returns permissions that a caller has on the specified resource.<br/>
> If the resource does not exist, this will return an empty set of<br/>
> permissions, not a NOT_FOUND error.

*Tags:* `projects`

#### Input Parameters
* `resource` - _required_ - REQUIRED: The resource for which the policy detail is being requested.
See the operation documentation for the appropriate value for this field.
* `access_token` - _optional_ - OAuth access token.
* `alt` - _optional_ - Data format for response.
    Possible values: json, media, proto.
* `callback` - _optional_ - JSONP
* `fields` - _optional_ - Selector specifying which fields to include in a partial response.
* `key` - _optional_ - API key. Your API key identifies your project and provides you with API access, quota, and reports. Required unless you provide an OAuth 2.0 token.
* `oauth_token` - _optional_ - OAuth 2.0 token for the current user.
* `prettyPrint` - _optional_ - Returns response with indentations and line breaks.
* `quotaUser` - _optional_ - Available to use for quota purposes for server-side applications. Can be any arbitrary string assigned to a user, but should not exceed 40 characters.
* `uploadType` - _optional_ - Legacy upload protocol for media (e.g. "media", "multipart").
* `upload_protocol` - _optional_ - Upload protocol for media (e.g. "raw", "multipart").

## License

**flow**ground :- Telekom iPaaS / googleapis-com-cloudiot-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
