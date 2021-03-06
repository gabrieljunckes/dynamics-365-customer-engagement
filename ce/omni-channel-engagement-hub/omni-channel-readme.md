---
title: "Known issues and limitations of  | MicrosoftDocs"
description: "Learn about the known issues and limitations in Omni-channel Engagement Hub."
keywords: ""
author: kabala123
ms.author: kabala
manager: shujoshi
applies_to: 
ms.date: 2/8/2019
ms.service: dynamics-365-customerservice
ms.topic: article
ms.assetid: BC3D3C77-982D-4F8F-B9DB-86854A1634F8
ms.custom: 
---

# Omni-channel Engagement Hub - Preview Readme (Known issues and Limitations)

Applies to Dynamics 365 for Customer Engagement apps version 9.1.0

[!include[cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]

The topic explains the known issues and limitations of Omni-channel Engagement Hub.

## Agents receive delayed notification when the chat ends
Customer ends the chat by selecting the Close (**X**) button on the chat widget. After the customer closes the chat, agent receives the notification of customer ending the conversation with a delay.

## Support for emojis
Emojis are not supported for the customer chat widget.

## Context variable support for duplicate and delete dependency check

While creating a context variable, the system does not perform duplicate detection in the work stream. Also, while deleting a context variable, the system does not perform a check for dependency.

## Screen pop decline or time out 
When an agent declines the screen pop or when the screen pop times out, work distribution mechanism puts a 2-minute pause on the agent’s clock and doesn’t allocate any new conversations to the agent for that time period.

## Queue configuration 
When you add a user to a queue, the sub grid doesn’t reflect the new member automatically. You are required to refresh the sub grid by selecting the **Refresh** button to see the new user in the list of queue members.

## Support for multiple channel providers
If your organization has deployed a third party channel provider using the Dynamics 365 Channel Integration Framework, and when you want to use Omni-channel Engagement Hub in the same organization, the Omni-channel solution overrides the Channel Integration Framework solution as there is no support for multiple channel providers.
 
## Support for knowledge articles when using Edge Process in Unified Service Desk
When you use Edge Process in Unified Service Desk, agents cannot open knowledge articles from knowledge Base search control.  
 
## Support for automatic record linking to conversation 
After agent creates a customer (contact/account) or case record using the quick create (+) option when in a session, it is not auto-linked to the conversation. As a workaround, agent can search for the newly created record using omni-channel search and link it to the conversation manually. 

## Dialog prompt in Unified Service Desk
When an agent logs on to Unified Service Desk client application, the client application shows a dialog to close the window. Agent must select **Yes** to proceed working in Unified Service Desk.

## Authentication error for different agent credentials
If agent is logged into Office 365 or Dynamics 365 through a different username in the browser (IE or Edge) than the one used for USD login, an authentication error is shown and user is not allowed to login. As a workaround, user should logout from all other accounts on the browser and try logging back in. 

## Transfer to queue does not show a message for the initiating agent 
When an agent initiates a transfer, the initiating agent becomes a consulting agent without any user interface message. However, the session tab name shows the **Consult** tag as the initiating agent is added to the same conversation as a consulting agent to enable smooth transition.
