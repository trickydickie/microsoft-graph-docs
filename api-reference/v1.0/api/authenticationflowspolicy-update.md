---
title: "Update authenticationFlowsPolicy"
description: "Update the Boolean selfServiceSignUp property of an authenticationFlowsPolicy object."
author: "linkhp"
localization_priority: Priority
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# Update authenticationFlowsPolicy

Namespace: microsoft.graph

Update the **selfServiceSignUp** property of an [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object. The properties **id**, **type**, and **description** cannot be modified.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|Policy.ReadWrite.AuthenticationFlows|
|Delegated (personal Microsoft account)|Not Supported|
|Application|Policy.ReadWrite.AuthenticationFlows|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/authenticationFlowsPolicy
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body

In the request body, you can supply a JSON representation of the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md) object.

The following table shows the properties that are required when you update the [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|selfServiceSignUp|[selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md)|Self-service sign-up configuration.|

## Response

If successful, this method returns a `204 No Content` response code and an empty response body.

## Example

### Request

<!-- {
  "blockType": "request",
  "name": "update_authenticationflowspolicy"
}
-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authenticationFlowsPolicy
Content-Type: application/json

{
  "selfServiceSignUp": {
    "isEnabled": true
  }
}
```

### Response

<!-- {
  "blockType": "response",
  "truncated": true
} -->

``` http
HTTP/1.1 204 No Content
```
