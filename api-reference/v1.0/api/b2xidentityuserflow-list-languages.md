---
title: "List languages"
description: "Retrieve a list of languages supported for customization within a B2X user flow."
author: "jkdouglas"
localization_priority: Normal
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# List languages

Namespace: microsoft.graph

Retrieve a list of languages supported for customization in a B2X user flow.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account)|IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All|
|Delegated (personal Microsoft account)| Not supported.|
|Application|IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All|

The work or school account needs to belong to one of the following roles:

* Global administrator
* External Identity User Flow administrator

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/languages
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) objects in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_2"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_PartnerSignUp/languages
```

### Response

**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguageConfiguration)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('B2X_1_PartnerSignUp')/languages",
  "value": [
    {
      "id": "en",
      "isEnabled": true,
      "displayName": "English"
    },
    {
      "id": "de",
      "isEnabled": true,
      "displayName": "Deutsch"
    }
  ]
}
```
