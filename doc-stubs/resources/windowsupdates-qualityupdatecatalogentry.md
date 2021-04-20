---
title: "qualityUpdateCatalogEntry resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# qualityUpdateCatalogEntry resource type

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [softwareUpdateCatalogEntry](../resources/windowsupdates-softwareupdatecatalogentry.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List qualityUpdateCatalogEntries](../api/windowsupdates-qualityupdatecatalogentry-list.md)|[microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md) collection|Get a list of the [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md) objects and their properties.|
|[Create qualityUpdateCatalogEntry](../api/windowsupdates-qualityupdatecatalogentry-create.md)|[microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md)|Create a new [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md) object.|
|[Get qualityUpdateCatalogEntry](../api/windowsupdates-qualityupdatecatalogentry-get.md)|[microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md)|Read the properties and relationships of a [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md) object.|
|[Update qualityUpdateCatalogEntry](../api/windowsupdates-qualityupdatecatalogentry-update.md)|[microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md)|Update the properties of a [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md) object.|
|[Delete qualityUpdateCatalogEntry](../api/windowsupdates-qualityupdatecatalogentry-delete.md)|None|Deletes a [qualityUpdateCatalogEntry](../resources/windowsupdates-qualityupdatecatalogentry.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deployableUntilDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [catalogEntry](../resources/windowsupdates-catalogentry.md).|
|displayName|String|**TODO: Add Description** Inherited from [catalogEntry](../resources/windowsupdates-catalogentry.md).|
|id|String|**TODO: Add Description** Inherited from [catalogEntry](../resources/windowsupdates-catalogentry.md).|
|isExpeditable|Boolean|**TODO: Add Description**|
|qualityUpdateClassification|qualityUpdateClassification|**TODO: Add Description**. Possible values are: `all`, `security`, `nonSecurity`, `unknownFutureValue`.|
|releaseDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [catalogEntry](../resources/windowsupdates-catalogentry.md).|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
  "baseType": "microsoft.graph.windowsUpdates.softwareUpdateCatalogEntry",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateCatalogEntry",
  "id": "String (identifier)",
  "displayName": "String",
  "deployableUntilDateTime": "String (timestamp)",
  "releaseDateTime": "String (timestamp)",
  "isExpeditable": "Boolean",
  "qualityUpdateClassification": "String"
}
```

