---
title: "Microsoft Dynamics 365 Customer Engagement msdyncrm_marketingconfiguration EntityType Reference | MicrosoftDocs"
ms.date: 07/10/2017
ms.service: "crm-online"
ms.topic: "reference"
applies_to: 
  - "Dynamics 365 (online)"
ms.assetid: 8f71e777-6be1-414b-94ad-26bfb406743e
author: "jimdaly"
ms.author: "jdaly"
manager: "jdaly"
meta-description: "Reference information about the Web API msdyncrm_marketingconfiguration entitytype."
---
# msdyncrm_marketingconfiguration EntityType
<table>
<tr><td><b>Description:</b></td><td>[!INCLUDE[./descriptions/msdyncrm_marketingconfiguration.md](./descriptions/msdyncrm_marketingconfiguration.md)]</td></tr>
<tr><td><b>Entity Set path:</b></td><td>[!include[current-web-api-base-uri.md](../includes/current-web-api-base-uri.md)]msdyncrm_marketingconfigurations </td></tr>
<tr><td><b>Base Type:</b></td><td>[crmbaseentity EntityType](crmbaseentity.md)</td></tr>
<tr><td><b>Display Name:</b></td><td>Marketing Configuration</td></tr>
<tr><td><b>Primary Key:</b></td><td>msdyncrm_marketingconfigurationid</td></tr>
<tr><td><b>Primary Name Attribute:</b></td><td>msdyncrm_name</td></tr>
<tr><td><b>Operations supported:</b></td><td>POST,GET,PATCH,DELETE</td></tr>
</table>
  
The msdyncrm_marketingconfiguration entitytype has no functions or actions bound to it.

## Properties
Properties represent fields of data stored in the entity. Some properties are read-only. 


|Name|Type|Details|  
|----|----|-------|  
|createdon|Edm.DateTimeOffset|**Display Name**: Created On<br />**Description**: Date and time when the record was created.<br />Read-only<br />|
|importsequencenumber|Edm.Int32|**Display Name**: Import Sequence Number<br />**Description**: Sequence number of the import that created this record.<br />|
|modifiedon|Edm.DateTimeOffset|**Display Name**: Modified On<br />**Description**: Date and time when the record was modified.<br />Read-only<br />|
|msdyncrm_configcacheexpirationdate|Edm.DateTimeOffset|**Display Name**: Config Cache Expiration Date<br />|
|msdyncrm_configcacheexpirationperiodinms|Edm.Int32|**Display Name**: Config Cache Expiration Period In Miliseconds<br />|
|msdyncrm_defaulttimezone|Edm.Int32|**Display Name**: Default Time Zone<br />|
|msdyncrm_enablelitmusintegration|Edm.Boolean|**Display Name**: Enable Litmus Integration<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>1</td><td>Yes</td></tr><tr><td>0</td><td>No</td></tr><tbody></table>|
|msdyncrm_marketingconfigurationid|Edm.Guid|**Display Name**: Marketing Configuration<br />**Description**: Unique identifier for entity instances<br />|
|msdyncrm_mktsvcdiscoveryendpointurl|Edm.String|**Display Name**: Marketing Service Discovery Endpoint Url<br />|
|msdyncrm_name|Edm.String|**Display Name**: Marketing Configuration<br />**Description**: The name of the Marketing Configuration entity.<br />|
|msdyncrm_organization_config|Edm.String|**Display Name**: Organization Config<br />**Description**: The configuration JSON<br />|
|msdyncrm_tokenauthenticationresource|Edm.String|**Display Name**: Token Authentication Resource<br />|
|msdyncrm_usebasicauth|Edm.Boolean|**Display Name**: Use Basic Auth<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>1</td><td>Yes</td></tr><tr><td>0</td><td>No</td></tr><tbody></table>|
|overriddencreatedon|Edm.DateTimeOffset|**Display Name**: Record Created On<br />**Description**: Date and time that the record was migrated.<br />|
|statecode|Edm.Int32|**Display Name**: Status<br />**Description**: Status of the Marketing Configuration<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>0</td><td>Active</td></tr><tr><td>1</td><td>Inactive</td></tr><tbody></table>|
|statuscode|Edm.Int32|**Display Name**: Status Reason<br />**Description**: Reason for the status of the Marketing Configuration<br />**Default Options**:<br /><table><thead><td>**Value**</td><td>**Label**</td></thead><tbody><tr><td>1</td><td>Active</td></tr><tr><td>2</td><td>Inactive</td></tr><tbody></table>|
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
|_msdyncrm_defaultcontact_value|msdyncrm_DefaultContact<br />||
|_msdyncrm_defaultcontentsettings_value|msdyncrm_DefaultContentSettings<br />||
|_organizationid_value|organizationid<br />|Unique identifier for the organization|


## Single-valued navigation properties
Single-valued navigation properties represent lookup fields where a single entity can be referenced. Each single-valued navigation property has a corresponding partner collection-valued navigation property on the related entity.


|Name|Type|Partner|  
|----|----|-------|  
|createdby|[systemuser EntityType](systemuser.md)|lk_msdyncrm_marketingconfiguration_createdby|
|createdonbehalfby|[systemuser EntityType](systemuser.md)|lk_msdyncrm_marketingconfiguration_createdonbehalfby|
|modifiedby|[systemuser EntityType](systemuser.md)|lk_msdyncrm_marketingconfiguration_modifiedby|
|modifiedonbehalfby|[systemuser EntityType](systemuser.md)|lk_msdyncrm_marketingconfiguration_modifiedonbehalfby|
|msdyncrm_DefaultContact|[contact EntityType](contact.md)|msdyncrm_contact_msdyncrm_marketingconfiguration_DefaultContact|
|msdyncrm_DefaultContentSettings|[msdyncrm_contentsettings EntityType](msdyncrm_contentsettings.md)|msdyncrm_msdyncrm_contentsettings_msdyncrm_marketingconfiguration_DefaultContentSettings|
|organizationid|[organization EntityType](organization.md)|organization_msdyncrm_marketingconfiguration|

## Collection-valued navigation properties
Collection-valued navigation properties represent collections of entities which may represent either a one-to-many (1:N) or many-to-many (N:N) relationship between the entities.


|Name|Type|Partner|  
|----|----|-------|  
|msdyncrm_marketingconfiguration_AsyncOperations|[asyncoperation EntityType](asyncoperation.md)|regardingobjectid_msdyncrm_marketingconfiguration|  
|msdyncrm_marketingconfiguration_BulkDeleteFailures|[bulkdeletefailure EntityType](bulkdeletefailure.md)|regardingobjectid_msdyncrm_marketingconfiguration|  
|msdyncrm_marketingconfiguration_DuplicateBaseRecord|[duplicaterecord EntityType](duplicaterecord.md)|baserecordid_msdyncrm_marketingconfiguration|  
|msdyncrm_marketingconfiguration_DuplicateMatchingRecord|[duplicaterecord EntityType](duplicaterecord.md)|duplicaterecordid_msdyncrm_marketingconfiguration|  
|msdyncrm_marketingconfiguration_SyncErrors|[syncerror EntityType](syncerror.md)|regardingobjectid_msdyncrm_marketingconfiguration|  

## Operations
The following operations can be used with the msdyncrm_marketingconfiguration entity type.


|Name|Binding|Description|  
|----|-------|-----------|  
|[IsValidStateTransition Function](../functions/isvalidstatetransition.md)|Not Bound|[!INCLUDE[../functions/descriptions/isvalidstatetransition.md](../functions/descriptions/isvalidstatetransition.md)]|  

## Solutions
The following solutions include the msdyncrm_marketingconfiguration entity type.


|Name|Description |  
|----|------------|  
|[Microsoft Dynamics Marketing Solution](../solutions/microsoftdynamicsmarketingcrmsolution.md)|[!INCLUDE[../solutions/descriptions/microsoftdynamicsmarketingcrmsolution.md](../solutions/descriptions/microsoftdynamicsmarketingcrmsolution.md)]|    

[!INCLUDE[./remarks/msdyncrm_marketingconfiguration.md](./remarks/msdyncrm_marketingconfiguration.md)]

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