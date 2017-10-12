---
title: "Microsoft Dynamics 365 Customer Engagement msdyncrm_linkedinactivity EntityType Reference | MicrosoftDocs"
ms.date: 07/10/2017
ms.service: "crm-online"
ms.topic: "reference"
applies_to: 
  - "Dynamics 365 (online)"
ms.assetid: 1bae84f5-24c0-443b-a87a-3a625002c6eb
author: "jimdaly"
ms.author: "jdaly"
manager: "jdaly"
meta-description: "Reference information about the Web API msdyncrm_linkedinactivity entitytype."
---
# msdyncrm_linkedinactivity EntityType
<table>
<tr><td><b>Description:</b></td><td>[!INCLUDE[./descriptions/msdyncrm_linkedinactivity.md](./descriptions/msdyncrm_linkedinactivity.md)]</td></tr>
<tr><td><b>Entity Set path:</b></td><td>[!include[current-web-api-base-uri.md](../includes/current-web-api-base-uri.md)]msdyncrm_linkedinactivities </td></tr>
<tr><td><b>Base Type:</b></td><td>[crmbaseentity EntityType](crmbaseentity.md)</td></tr>
<tr><td><b>Display Name:</b></td><td>LinkedIn Activity</td></tr>
<tr><td><b>Primary Key:</b></td><td>msdyncrm_linkedinactivityid</td></tr>
<tr><td><b>Primary Name Attribute:</b></td><td>msdyncrm_name</td></tr>
<tr><td><b>Operations supported:</b></td><td>POST,GET,PATCH,DELETE</td></tr>
</table>
  
The msdyncrm_linkedinactivity entitytype has no functions or actions bound to it.

## Properties
Properties represent fields of data stored in the entity. Some properties are read-only. 


|Name|Type|Details|  
|----|----|-------|  
|createdon|Edm.DateTimeOffset|**Display Name**: Created On<br />**Description**: Date and time when the record was created.<br />Read-only<br />|
|importsequencenumber|Edm.Int32|**Display Name**: Import Sequence Number<br />**Description**: Sequence number of the import that created this record.<br />|
|modifiedon|Edm.DateTimeOffset|**Display Name**: Modified On<br />**Description**: Date and time when the record was modified.<br />Read-only<br />|
|msdyncrm_action_status|Edm.String|**Display Name**: Action Status<br />**Description**: The status of Marketing Activity creation<br />|
|msdyncrm_activityadditionalparams|Edm.String|**Display Name**: JSON Payload<br />|
|msdyncrm_actualdurationminutes|Edm.Int32|**Display Name**: Actual duration in minutes<br />|
|msdyncrm_actualend|Edm.DateTimeOffset|**Display Name**: Actual end<br />|
|msdyncrm_actualstart|Edm.DateTimeOffset|**Display Name**: Actual start<br />|
|msdyncrm_description|Edm.String|**Display Name**: Description<br />|
|msdyncrm_durationmillisecond|Edm.Int32|**Display Name**: Duration in milliseconds<br />|
|msdyncrm_error_message|Edm.String|**Display Name**: Error message<br />|
|msdyncrm_linkedinactivityid|Edm.Guid|**Display Name**: LinkedIn Activity<br />**Description**: Unique identifier for entity instances<br />|
|msdyncrm_name|Edm.String|**Display Name**: Name<br />**Description**: The name of the custom entity.<br />|
|overriddencreatedon|Edm.DateTimeOffset|**Display Name**: Record Created On<br />**Description**: Date and time that the record was migrated.<br />|
|statecode|Edm.Int32|**Display Name**: Status<br />**Description**: Status of the LinkedIn Activity<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>0</td><td>Active</td></tr><tr><td>1</td><td>Inactive</td></tr><tbody></table>|
|statuscode|Edm.Int32|**Display Name**: Status Reason<br />**Description**: Reason for the status of the LinkedIn Activity<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>1</td><td>Active</td></tr><tr><td>2</td><td>Inactive</td></tr><tbody></table>|
|timezoneruleversionnumber|Edm.Int32|**Display Name**: Time Zone Rule Version Number<br />**Description**: For internal use only.<br />|
|utcconversiontimezonecode|Edm.Int32|**Display Name**: UTC Conversion Time Zone Code<br />**Description**: Time zone code that was in use when the record was created.<br />|
|versionnumber|Edm.Int64|**Display Name**: Version Number<br />**Description**: Version Number<br />Read-only<br />|

## Lookup Properties
Lookup properties are read-only, computed properties which contain entity primary key Edm.Guid data for one or more corresponding single-valued navigation properties. More information: [Lookup properties](https://msdn.microsoft.com/library/mt607990.aspx#bkmk_lookupProperties) and [Retrieve data about lookup properties](https://msdn.microsoft.com/library/gg334767.aspx#bkmk_lookupProperty).


|Name|Single-valued navigation property|Description|  
|----|---------------------------------|-----------|  
|_createdby_value|createdby<br />|Unique identifier of the user who created the record.|
|_createdonbehalfby_value|createdonbehalfby<br />|Unique identifier of the delegate user who created the record.|
|_modifiedby_value|modifiedby<br />|Unique identifier of the user who modified the record.|
|_modifiedonbehalfby_value|modifiedonbehalfby<br />|Unique identifier of the delegate user who modified the record.|
|_ownerid_value|ownerid<br />|Owner Id|
|_owningbusinessunit_value|owningbusinessunit<br />|Unique identifier for the business unit that owns the record|
|_owningteam_value|owningteam<br />|Unique identifier for the team that owns the record.|
|_owninguser_value|owninguser<br />|Unique identifier for the user that owns the record.|


## Single-valued navigation properties
Single-valued navigation properties represent lookup fields where a single entity can be referenced. Each single-valued navigation property has a corresponding partner collection-valued navigation property on the related entity.


|Name|Type|Partner|  
|----|----|-------|  
|createdby|[systemuser EntityType](systemuser.md)|lk_msdyncrm_linkedinactivity_createdby|
|createdonbehalfby|[systemuser EntityType](systemuser.md)|lk_msdyncrm_linkedinactivity_createdonbehalfby|
|modifiedby|[systemuser EntityType](systemuser.md)|lk_msdyncrm_linkedinactivity_modifiedby|
|modifiedonbehalfby|[systemuser EntityType](systemuser.md)|lk_msdyncrm_linkedinactivity_modifiedonbehalfby|
|ownerid|[principal EntityType](principal.md)|owner_msdyncrm_linkedinactivity|
|owningbusinessunit|[businessunit EntityType](businessunit.md)|business_unit_msdyncrm_linkedinactivity|
|owningteam|[team EntityType](team.md)|team_msdyncrm_linkedinactivity|
|owninguser|[systemuser EntityType](systemuser.md)|user_msdyncrm_linkedinactivity|

## Collection-valued navigation properties
Collection-valued navigation properties represent collections of entities which may represent either a one-to-many (1:N) or many-to-many (N:N) relationship between the entities.


|Name|Type|Partner|  
|----|----|-------|  
|msdyncrm_linkedinactivity_ActivityPointers|[activitypointer EntityType](activitypointer.md)|regardingobjectid_msdyncrm_linkedinactivity|  
|msdyncrm_linkedinactivity_adx_alertsubscriptions|[adx_alertsubscription EntityType](adx_alertsubscription.md)|regardingobjectid_msdyncrm_linkedinactivity_adx_alertsubscription|  
|msdyncrm_linkedinactivity_adx_inviteredemptions|[adx_inviteredemption EntityType](adx_inviteredemption.md)|regardingobjectid_msdyncrm_linkedinactivity_adx_inviteredemption|  
|msdyncrm_linkedinactivity_adx_portalcomments|[adx_portalcomment EntityType](adx_portalcomment.md)|regardingobjectid_msdyncrm_linkedinactivity_adx_portalcomment|  
|msdyncrm_linkedinactivity_Annotations|[annotation EntityType](annotation.md)|objectid_msdyncrm_linkedinactivity|  
|msdyncrm_linkedinactivity_Appointments|[appointment EntityType](appointment.md)|regardingobjectid_msdyncrm_linkedinactivity_appointment|  
|msdyncrm_linkedinactivity_AsyncOperations|[asyncoperation EntityType](asyncoperation.md)|regardingobjectid_msdyncrm_linkedinactivity|  
|msdyncrm_linkedinactivity_BulkDeleteFailures|[bulkdeletefailure EntityType](bulkdeletefailure.md)|regardingobjectid_msdyncrm_linkedinactivity|  
|msdyncrm_linkedinactivity_connections1|[connection EntityType](connection.md)|record1id_msdyncrm_linkedinactivity|  
|msdyncrm_linkedinactivity_connections2|[connection EntityType](connection.md)|record2id_msdyncrm_linkedinactivity|  
|msdyncrm_linkedinactivity_DuplicateBaseRecord|[duplicaterecord EntityType](duplicaterecord.md)|baserecordid_msdyncrm_linkedinactivity|  
|msdyncrm_linkedinactivity_DuplicateMatchingRecord|[duplicaterecord EntityType](duplicaterecord.md)|duplicaterecordid_msdyncrm_linkedinactivity|  
|msdyncrm_linkedinactivity_Emails|[email EntityType](email.md)|regardingobjectid_msdyncrm_linkedinactivity_email|  
|msdyncrm_linkedinactivity_Faxes|[fax EntityType](fax.md)|regardingobjectid_msdyncrm_linkedinactivity_fax|  
|msdyncrm_linkedinactivity_Feedback|[feedback EntityType](feedback.md)|regardingobjectid_msdyncrm_linkedinactivity|  
|msdyncrm_linkedinactivity_Letters|[letter EntityType](letter.md)|regardingobjectid_msdyncrm_linkedinactivity_letter|  
|msdyncrm_linkedinactivity_msdyn_approvals|[msdyn_approval EntityType](msdyn_approval.md)|regardingobjectid_msdyncrm_linkedinactivity_msdyn_approval|  
|msdyncrm_linkedinactivity_msdyn_bookingalerts|[msdyn_bookingalert EntityType](msdyn_bookingalert.md)|regardingobjectid_msdyncrm_linkedinactivity_msdyn_bookingalert|  
|msdyncrm_linkedinactivity_msdyn_surveyinvites|[msdyn_surveyinvite EntityType](msdyn_surveyinvite.md)|regardingobjectid_msdyncrm_linkedinactivity_msdyn_surveyinvite|  
|msdyncrm_linkedinactivity_PhoneCalls|[phonecall EntityType](phonecall.md)|regardingobjectid_msdyncrm_linkedinactivity_phonecall|  
|msdyncrm_linkedinactivity_RecurringAppointmentMasters|[recurringappointmentmaster EntityType](recurringappointmentmaster.md)|regardingobjectid_msdyncrm_linkedinactivity_recurringappointmentmaster|  
|msdyncrm_linkedinactivity_ServiceAppointments|[serviceappointment EntityType](serviceappointment.md)|regardingobjectid_msdyncrm_linkedinactivity_serviceappointment|  
|msdyncrm_linkedinactivity_SocialActivities|[socialactivity EntityType](socialactivity.md)|regardingobjectid_msdyncrm_linkedinactivity_socialactivity|  
|msdyncrm_linkedinactivity_SyncErrors|[syncerror EntityType](syncerror.md)|regardingobjectid_msdyncrm_linkedinactivity|  
|msdyncrm_linkedinactivity_Tasks|[task EntityType](task.md)|regardingobjectid_msdyncrm_linkedinactivity_task|  

## Operations
The following operations can be used with the msdyncrm_linkedinactivity entity type.


|Name|Binding|Description|  
|----|-------|-----------|  
|[GrantAccess Action](../actions/grantaccess.md)|Not Bound|[!INCLUDE[../actions/descriptions/grantaccess.md](../actions/descriptions/grantaccess.md)]|  
|[IsValidStateTransition Function](../functions/isvalidstatetransition.md)|Not Bound|[!INCLUDE[../functions/descriptions/isvalidstatetransition.md](../functions/descriptions/isvalidstatetransition.md)]|  
|[ModifyAccess Action](../actions/modifyaccess.md)|Not Bound|[!INCLUDE[../actions/descriptions/modifyaccess.md](../actions/descriptions/modifyaccess.md)]|  
|[RetrievePrincipalAccess Function](../functions/retrieveprincipalaccess.md)|Not Bound|[!INCLUDE[../functions/descriptions/retrieveprincipalaccess.md](../functions/descriptions/retrieveprincipalaccess.md)]|  
|[RetrieveSharedPrincipalsAndAccess Function](../functions/retrievesharedprincipalsandaccess.md)|Not Bound|[!INCLUDE[../functions/descriptions/retrievesharedprincipalsandaccess.md](../functions/descriptions/retrievesharedprincipalsandaccess.md)]|  
|[RevokeAccess Action](../actions/revokeaccess.md)|Not Bound|[!INCLUDE[../actions/descriptions/revokeaccess.md](../actions/descriptions/revokeaccess.md)]|  

## Solutions
The following solutions include the msdyncrm_linkedinactivity entity type.


|Name|Description |  
|----|------------|  
|[LinkedIn Lead Gen Forms Solution](../solutions/linkedinleadgenintegration.md)|[!INCLUDE[../solutions/descriptions/linkedinleadgenintegration.md](../solutions/descriptions/linkedinleadgenintegration.md)]|    

[!INCLUDE[./remarks/msdyncrm_linkedinactivity.md](./remarks/msdyncrm_linkedinactivity.md)]

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