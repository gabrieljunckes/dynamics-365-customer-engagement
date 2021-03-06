---
title: "Solution tools for team development (Developer Guide for Dynamics 365 for Customer Engagement apps)| MicrosoftDocs"
description: "This topic gives details about tools that can be used for team development of Dynamics 365 for Customer Engagement solutions and for source code control"
ms.custom: 
ms.date: 10/31/2017
ms.reviewer: 
ms.service: crm-online
ms.suite: 
ms.tgt_pltfrm: 
ms.topic: article
applies_to: 
  - Dynamics 365 for Customer Engagement (online)
ms.assetid: af0cb38e-58f4-4aa6-82c4-da67f07115f9
caps.latest.revision: 17
author: JimDaly
ms.author: jdaly
manager: amyla
search.audienceType: 
  - developer
search.app: 
  - D365CE
---
# Solution tools for team development

[!INCLUDE[](../includes/cc_applies_to_update_9_0_0.md)]

A [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] solution is a compressed (.zip) file that contains multiple customized components that have been exported from a [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] server so that they may be transported and imported into another server. However, a solution file is a single binary file that does not lend itself to source code control or team development. There is no way for multiple developers to work on the custom components in the solution.  
  
 The SolutionPackager tool resolves the problem of source code control and team development of solution files. The tool identifies individual components in the compressed solution file and extracts them out to individual files. The tool can also re-create a solution file by packing the files that had been previously extracted. This enables multiple people to work independently on a single solution and extract their changes into a common location. Because each component in the solution file is broken into multiple files, it becomes possible to merge customizations without overwriting prior changes. A secondary use of the SolutionPackager tool is that it can be invoked from an automated build process to generate a compressed solution file from previously extracted component files without needing an active [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] server.

 The SolutionPackager tool is distributed as part of the [Microsoft.CrmSdk.CoreTools](https://www.nuget.org/packages/Microsoft.CrmSdk.CoreTools) NuGet package. See [Download tools from NuGet](download-tools-nuget.md) for information about how to download it.
  
## In This Section  
 [Use the SolutionPackager Tool to Compress and Extract a Solution File](compress-extract-solution-file-solutionpackager.md)  
  
 [Use Source Control with Solution Files](use-source-control-solution-files.md)  
  
 [Solution Component File Reference (SolutionPackager)](solution-component-file-reference-solutionpackager.md)  
  
## Related Sections  
 [Developer Tools](developer-tools.md)  
  
 [Package and Distribute Extensions with Dynamics 365 for Customer Engagement Solutions](package-distribute-extensions-use-solutions.md)
