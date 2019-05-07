# ![LOGO](logo.png) StorageImportExport **flow**ground Connector

## Description

A generated **flow**ground connector for the StorageImportExport API (version 2016-11-01).

Generated from: https://api.apis.guru/v2/specs/azure.com/storageimportexport/2016-11-01/swagger.json<br/>
Generated at: 2019-05-07T17:39:16+03:00

## API Description

The Storage Import/Export Resource Provider API.

## Authorization

Supported authorization schemes:
- OAuth2

For OAuth 2.0 you need to specify OAuth Client credentials as environment variables in the connector repository:
* `OAUTH_CLIENT_ID` - your OAuth client id
* `OAUTH_CLIENT_SECRET` - your OAuth client secret

## Actions

### Returns a list of locations to which you can ship the disks associated with an import or export job. A location is a Microsoft data center region.

*Tags:* `StorageImportExport`

#### Input Parameters
* `api-version` - _required_ - Specifies the API version to use for this request.
    Possible values: 2016-11-01.
* `Accept-Language` - _optional_ - Specifies the preferred language for the response.

### Returns the details about a location to which you can ship the disks associated with an import or export job. A location is an Azure region.

*Tags:* `StorageImportExport`

#### Input Parameters
* `locationName` - _required_ - The name of the location. For example, West US or westus.
* `api-version` - _required_ - Specifies the API version to use for this request.
    Possible values: 2016-11-01.
* `Accept-Language` - _optional_ - Specifies the preferred language for the response.

### Returns the list of operations supported by the import/export resource provider.

*Tags:* `StorageImportExport`

#### Input Parameters
* `api-version` - _required_ - Specifies the API version to use for this request.
    Possible values: 2016-11-01.
* `Accept-Language` - _optional_ - Specifies the preferred language for the response.

### Returns all active and completed jobs in a subscription.

*Tags:* `StorageImportExport`

#### Input Parameters
* `$top` - _optional_ - An integer value that specifies how many jobs at most should be returned. The value cannot exceed 100.
* `$filter` - _optional_ - Can be used to restrict the results to certain conditions.
* `subscriptionId` - _required_ - The subscription ID for the Azure user.
* `api-version` - _required_ - Specifies the API version to use for this request.
    Possible values: 2016-11-01.
* `Accept-Language` - _optional_ - Specifies the preferred language for the response.

### Returns all active and completed jobs in a resource group.

*Tags:* `StorageImportExport`

#### Input Parameters
* `$top` - _optional_ - An integer value that specifies how many jobs at most should be returned. The value cannot exceed 100.
* `$filter` - _optional_ - Can be used to restrict the results to certain conditions.
* `subscriptionId` - _required_ - The subscription ID for the Azure user.
* `resourceGroupName` - _required_ - The resource group name uniquely identifies the resource group within the user subscription.
* `api-version` - _required_ - Specifies the API version to use for this request.
    Possible values: 2016-11-01.
* `Accept-Language` - _optional_ - Specifies the preferred language for the response.

### Deletes an existing job. Only jobs in the Creating or Completed states can be deleted.

*Tags:* `StorageImportExport`

#### Input Parameters
* `jobName` - _required_ - The name of the import/export job.
* `subscriptionId` - _required_ - The subscription ID for the Azure user.
* `resourceGroupName` - _required_ - The resource group name uniquely identifies the resource group within the user subscription.
* `api-version` - _required_ - Specifies the API version to use for this request.
    Possible values: 2016-11-01.
* `Accept-Language` - _optional_ - Specifies the preferred language for the response.

### Gets information about an existing job.

*Tags:* `StorageImportExport`

#### Input Parameters
* `jobName` - _required_ - The name of the import/export job.
* `subscriptionId` - _required_ - The subscription ID for the Azure user.
* `resourceGroupName` - _required_ - The resource group name uniquely identifies the resource group within the user subscription.
* `api-version` - _required_ - Specifies the API version to use for this request.
    Possible values: 2016-11-01.
* `Accept-Language` - _optional_ - Specifies the preferred language for the response.

### Updates specific properties of a job. You can call this operation to notify the Import/Export service that the hard drives comprising the import or export job have been shipped to the Microsoft data center. It can also be used to cancel an existing job.

*Tags:* `StorageImportExport`

#### Input Parameters
* `jobName` - _required_ - The name of the import/export job.
* `subscriptionId` - _required_ - The subscription ID for the Azure user.
* `resourceGroupName` - _required_ - The resource group name uniquely identifies the resource group within the user subscription.
* `api-version` - _required_ - Specifies the API version to use for this request.
    Possible values: 2016-11-01.
* `Accept-Language` - _optional_ - Specifies the preferred language for the response.

### Creates a new job or updates an existing job in the specified subscription.

*Tags:* `StorageImportExport`

#### Input Parameters
* `jobName` - _required_ - The name of the import/export job.
* `subscriptionId` - _required_ - The subscription ID for the Azure user.
* `resourceGroupName` - _required_ - The resource group name uniquely identifies the resource group within the user subscription.
* `api-version` - _required_ - Specifies the API version to use for this request.
    Possible values: 2016-11-01.
* `Accept-Language` - _optional_ - Specifies the preferred language for the response.
* `x-ms-client-tenant-id` - _optional_ - The tenant ID of the client making the request.

### Returns the BitLocker Keys for all drives in the specified job.

*Tags:* `StorageImportExport`

#### Input Parameters
* `jobName` - _required_ - The name of the import/export job.
* `subscriptionId` - _required_ - The subscription ID for the Azure user.
* `resourceGroupName` - _required_ - The resource group name uniquely identifies the resource group within the user subscription.
* `api-version` - _required_ - Specifies the API version to use for this request.
    Possible values: 2016-11-01.
* `Accept-Language` - _optional_ - Specifies the preferred language for the response.

## License

**flow**ground :- Telekom iPaaS / azure-com-storageimportexport-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
