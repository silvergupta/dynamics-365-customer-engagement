---
title: "OnOrAfter Query Function | MicrosoftDocs"
ms.date: "2017-07-10"
ms.service: "crm-online"
ms.topic: "reference"
applies_to: 
  - "Dynamics 365 (online)"
ms.assetid: 9f356a75-a47b-4e40-9334-7323bc1a68c8
author: "jimdaly"
ms.author: "jdaly"
manager: "jdaly"
---
# OnOrAfter Function
[!INCLUDE[./descriptions/onorafter.md](./descriptions/onorafter.md)]  
  
|Name|Type|Nullable|Unicode|Description|  
|----------|----------|--------------|-------------|-----------------|  
|PropertyName|Edm.String|false|false|The name of the property to evaluate. |
|PropertyValue|Edm.String|false|false|The value to compare. | 


## Syntax example
`?$filter=Microsoft.Dynamics.CRM.OnOrAfter(PropertyName=@p1,PropertyValue=@p2)&@p1='name'&@p2='value'`
 
[!INCLUDE[./remarks/onorafter.md](./remarks/onorafter.md)]

### See also  
 [Use the Microsoft Dynamics CRM Web API](https://msdn.microsoft.com/library/mt593051.aspx)<br />
 [Web API EntityType Reference](../entitytypereference.md)<br />
 [Web API Action Reference](../actionreference.md)<br />
 [Web API Function Reference](../functionreference.md)<br />
 [Web API Query Function Reference](../queryfunctionreference.md)<br />
 [Web API EnumType Reference](../enumtypereference.md)<br />
 [Web API ComplexType Reference](../complextypereference.md)<br />
 [Web API Metadata EntityType Reference](../entitytypereference.md)<br />
 [Web API Solutions Reference](../solutionreference.md)<br />