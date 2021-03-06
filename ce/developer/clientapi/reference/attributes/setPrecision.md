---
title: "setPrecision (Client API reference) in Dynamics 365 for Customer Engagement| MicrosoftDocs"
ms.date: 10/31/2017
ms.service: crm-online
ms.topic: reference
applies_to: Dynamics 365 for Customer Engagement (online)
ms.assetid: 580aebec-c1d1-4e4a-8c20-ced859569fb2
author: KumarVivek
ms.author: kvivek
manager: amyla
search.audienceType: 
  - developer
search.app: 
  - D365CE
---
# setPrecision (Client API reference)

[!INCLUDE[](../../../../includes/cc_applies_to_update_9_0_0.md)]

Sets the number of digits allowed to the right of the decimal point. 

## Attribute types supported

Money, decimal, double, and integer

## Syntax

`formContext.getAttribute(arg).setPrecision(value);`

## Parameter

 Parameter Name| Type| Description  |
| --------|-----------| -----|
|value| Number| Number of digits allowed to the right of the decimal point.|

### Related topics

[getPrecision](getPrecision.md)

