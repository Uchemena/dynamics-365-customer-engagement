---
title: Connect using a new Azure resource 
description: Use this article to understand how to connect to Azure Communication Services using a new Azure resource in Customer Service admin center.
ms.date: 05/31/2024
ms.topic: article
author: neeranelli
ms.author: nenellim
---
# Quickstart: Connect using a new Azure resource

[!INCLUDE[cc-use-with-omnichannel](../../includes/cc-use-with-omnichannel.md)]

In the voice channel, you can quickly connect to Azure Communication Services, provision phone numbers, and set up outbound and inbound calling for your business by creating and deploying a new Azure resource. More information: [Azure Communication Services](/azure/communication-services/overview)

## Prerequisites

Before you connect an Azure resource to Azure Communication Services, you must perform the following steps.

- Check whether the **Get started** button to connect to an existing Azure resource is visible on the **Phone numbers** page. The **Get Started** button appears only in the following scenarios.
    - The trial has ended after the free calling time has elapsed.
    - You've manually ended the trial.
    - You've disconnected from the Azure resource. More information: [Disconnect from Azure Communication Services resource](voice-channel-disconnect-from-acs.md)
- Have an Azure subscription that's in the same tenant as your Dynamics 365 account. Ensure that your Azure subscription meets the [Subscription eligibility and number capabilities](/azure/communication-services/concepts/numbers/sub-eligibility-number-capability) requirements.
- Have at least contributor-level permissions to the Azure subscription. To check your role, open your subscription and view the **My role** column of your subscription on the Azure portal. You'll be able to deploy your Azure Communication Services resource only if you have contributor-level permissions.
 
## Connect using a new Azure resource

1. In the site map of Customer Service admin center, select **Channels** in **Customer support**. The **Channels** page appears.

1. Select **Manage** for **Phone numbers**.

1. Select **Get started**. The **Connect to Azure Communication Services** dialog opens.

1. Select **Create new resource** and enter the following details.
   - **Azure subscription**: Select a subscription from the dropdown list.
   - **Azure resource group**: Select an existing resource group or select **Create new**, and enter a name for a new resource group.
      > [!NOTE]
      > The resource group name should be unique within a subscription.
   - **Resource name**: Enter a name for the resource. The resource name can contain only letters, numbers, and hyphens.
1. Select **Deploy** to create and deploy the resource.

Your new Azure resource is connected to Azure Communication Services. You can now [acquire new phone numbers](voice-channel-manage-phone-numbers.md) for your organization via the new resource and also [enable call recording and SMS services](voice-channel-connect-existing-resource.md#enable-incoming-calls-call-recording-and-sms-services).

### See also

[Overview of the voice channel](voice-channel.md)  
[Manage phone numbers](voice-channel-manage-phone-numbers.md)  
[Connect to Azure Communication Services](voice-channel-acs-resource.md)  
[Connect using an existing Azure resource](voice-channel-connect-existing-resource.md)  
[Disconnect from Azure Communication Services](voice-channel-disconnect-from-acs.md)  
[Set up outbound calling](voice-channel-outbound-calling.md)  
[Set up inbound calling](../voice-channel-route-queues.md)  
[Bring your own carrier](voice-channel-bring-your-own-number.md)  
[Integrate third-party IVR systems with voice channel](voice-channel-contextual-transfer-external-ivr.md)   
[Import phone numbers](voice-channel-sync-from-acs.md)  

[!INCLUDE[footer-include](../../includes/footer-banner.md)]