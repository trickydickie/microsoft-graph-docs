---
title: "Update catalogEntry"
description: "Update the properties of a catalogEntry object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update catalogEntry
Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [catalogEntry](../resources/windowsupdates-catalogentry.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /admin/windows/updates/catalog/entries/{catalogEntryId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [catalogEntry](../resources/windowsupdates-catalogentry.md) object.

The following table shows the properties that are required when you update the [catalogEntry](../resources/windowsupdates-catalogentry.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|deployableUntilDateTime|DateTimeOffset|**TODO: Add Description**|
|releaseDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [catalogEntry](../resources/windowsupdates-catalogentry.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_catalogentry"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/admin/windows/updates/catalog/entries/{catalogEntryId}
Content-Type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.windowsUpdates.catalogEntry",
  "displayName": "String",
  "deployableUntilDateTime": "String (timestamp)",
  "releaseDateTime": "String (timestamp)"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.catalogEntry",
  "id": "c9386bb8-6bb8-c938-b86b-38c9b86b38c9",
  "displayName": "String",
  "deployableUntilDateTime": "String (timestamp)",
  "releaseDateTime": "String (timestamp)"
}
```

