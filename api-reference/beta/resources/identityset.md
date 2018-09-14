---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: IdentitySet
---
# IdentitySet resource type

> **Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change. Use of these APIs in production applications is not supported.

The **IdentitySet** resource is a keyed collection of [Identity](identity.md) resources.
It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.

## Properties

| Property            | Type                    | Description                                                     |
|:--------------------|:------------------------|:----------------------------------------------------------------|
| application         | [identity](identity.md) | Optional. The application associated with this action.          |
| applicationInstance | [identity](identity.md) | Optional. The application instance associated with this action. |
| device              | [identity](identity.md) | Optional. The device associated with this action.                
| phone               | [identity](identity.md) | Optional. The phone number associated with this action.          
| user                | [identity](identity.md) | Optional. The user associated with this action.                  

## JSON representation

Here is a JSON representation of the resource.

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identitySet",
       "optionalProperties": ["user", "application", "applicationInstance", "device", "phone"],
       "openType": true } -->

```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "phone": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## Remarks

See [DriveItem](driveitem.md) for usage of **IdentitySet** resources. 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->