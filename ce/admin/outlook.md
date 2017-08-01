---
title: "Dynamics 365 for Outlook | MicrosoftDocs"
ms.custom: ""
ms.date: "2017-08-31"
ms.reviewer: ""
ms.service: "crm-online"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
applies_to: 
  - "Dynamics 365 (online)"
  - "Dynamics 365 Version 9.x"
ms.assetid: ae7a0418-73fc-476f-8fa5-dc6505273ea1
caps.latest.revision: 13
author: "jimholtz"
ms.author: "jimholtz"
manager: "brycho"
---
# Dynamics 365 for Outlook
<a name="BKMK_Outlooksync"></a> [!INCLUDE[pn_crm_for_outlook_full](../includes/pn-crm-for-outlook-full.md)] can synchronize email messages, contacts, tasks, and appointments between [!INCLUDE[pn_MS_Outlook_Full](../includes/pn-ms-outlook-full.md)] and [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)] (client-to-server synchronization). Similar to [!INCLUDE[cc_server_side_synch](../includes/cc-server-side-synch.md)], synchronization filters are used to synchronize messaging data from [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)] to [!INCLUDE[pn_Outlook_short](../includes/pn-outlook-short.md)] or [!INCLUDE[pn_Exchange](../includes/pn-exchange.md)]. Manually tracked or Inbox-rule based tracking is used to synchronize messaging data from [!INCLUDE[pn_Exchange](../includes/pn-exchange.md)] or [!INCLUDE[pn_Outlook_short](../includes/pn-outlook-short.md)] to [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)].  
  
 ![Dynamics 365 for Outlook synchronization](../admin/media/crm-outlook-sync.png "Dynamics 365 for Outlook synchronization")  
  
 When you use [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)], there are a few synchronization concepts that are helpful to understand. Notice that, to have any of this [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)] functionality, each [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)] user must run the [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)] add-in and the [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)] user mailbox record must be configured appropriately.  
  
 When you select [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)] as the messaging data synchronization method in the user mailbox record, email, contacts, appointments, and tasks created in [!INCLUDE[pn_Outlook_short](../includes/pn-outlook-short.md)] are synchronized with [!INCLUDE[pn_CRM_Online](../includes/pn-crm-online.md)] or [!INCLUDE[pn_crm_op_edition](../includes/pn-crm-op-edition.md)].  
  
## Dynamics 365 for Outlook synchronization concepts  
 Note the following concepts when you use [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)] as the synchronizing agent:  
  
1. **Synchronizing organization**. Only one organization can be designated as the synchronizing organization. If you have more than one [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)] organization configured, you can view the synchronizing organization in the [!INCLUDE[pn_Configuration_Wizard_long](../includes/pn-configuration-wizard-long.md)]. The [!INCLUDE[pn_configuration_wizard](../includes/pn-configuration-wizard.md)] is an application included with [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)]. Notice that you can still connect to additional organizations by using [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)]. However, when an organization is not defined as the synchronizing organization in [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)], messaging data in [!INCLUDE[pn_Outlook_short](../includes/pn-outlook-short.md)] does not synchronize with that organization.  
  
2. **Synchronizing mailbox**. Only one [!INCLUDE[pn_Exchange](../includes/pn-exchange.md)] or POP3 mailbox can be designated for a single [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)] user. You cannot designate multiple mailboxes and you cannot map more than one [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)] user to a single [!INCLUDE[pn_Exchange](../includes/pn-exchange.md)] or POP3 email mailbox. This mailbox is referred to as the primary mailbox.  
  
3. **Synchronizing Dynamics 365 for Outlook instance**. Only one [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)] instance can be designated as the Synchronizing [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)] instance. When you sign-in to an organization from another PC that is running [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)] that is not the synchronizing [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)] instance you will receive a dialog message asking whether you want to designate the current [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)] instance as the synchronizing [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)] instance. Notice that, when you choose not to set the [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)] instance as the synchronizing instance, you can still connect to the [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)] organization and perform tasks, but messaging data in [!INCLUDE[pn_Outlook_short](../includes/pn-outlook-short.md)] will not synchronize with the [!INCLUDE[pn_microsoftcrm](../includes/pn-microsoftcrm.md)] organization.  
  
4. **Go Offline data sync**. Go offline capability uses [!INCLUDE[pn_ms_SQL_Server_Express_long](../includes/pn-ms-sql-server-express-long.md)] as the local data store. When you go offline or come back online, [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)] synchronizes the records for the entity types you choose with the [!INCLUDE[pn_CRM_Online](../includes/pn-crm-online.md)] or [!INCLUDE[pn_crm_op_edition](../includes/pn-crm-op-edition.md)]. When you go offline or come back online, a separate synchronization process takes place that is not part of the messaging data synchronization described here. Go offline capability allows users to create, modify, or delete records offline that can be later synchronized to [!INCLUDE[pn_CRM_Online](../includes/pn-crm-online.md)] or [!INCLUDE[pn_crm_op_edition](../includes/pn-crm-op-edition.md)] when [!INCLUDE[pn_crm_for_outlook_short](../includes/pn-crm-for-outlook-short.md)] comes online again.  
  
### See also  
 [Set up Dynamics 365 for Outlook](../admin/set-up-outlook.md)   
 [Synchronizing data with Outlook or Exchange FAQ](http://go.microsoft.com/fwlink/p/?LinkID=518288)