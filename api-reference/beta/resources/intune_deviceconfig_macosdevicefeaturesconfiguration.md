﻿# macOSDeviceFeaturesConfiguration resource type

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

MacOS device features configuration profile.

Inherits from [appleDeviceFeaturesConfigurationBase](../resources/intune_deviceconfig_appledevicefeaturesconfigurationbase.md)

## Methods
|Method|Return Type|Description|
|---|---|---|
|[List macOSDeviceFeaturesConfigurations](../api/intune_deviceconfig_macosdevicefeaturesconfiguration_list.md)|[macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) collection|List properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) objects.|
|[Get macOSDeviceFeaturesConfiguration](../api/intune_deviceconfig_macosdevicefeaturesconfiguration_get.md)|[macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md)|Read properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object.|
|[Create macOSDeviceFeaturesConfiguration](../api/intune_deviceconfig_macosdevicefeaturesconfiguration_create.md)|[macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md)|Create a new [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object.|
|[Delete macOSDeviceFeaturesConfiguration](../api/intune_deviceconfig_macosdevicefeaturesconfiguration_delete.md)|None|Deletes a [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md).|
|[Update macOSDeviceFeaturesConfiguration](../api/intune_deviceconfig_macosdevicefeaturesconfiguration_update.md)|[macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md)|Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune_deviceconfig_macosdevicefeaturesconfiguration.md) object.|
|[List deviceConfigurationGroupAssignments](../api/intune_deviceconfig_macosdevicefeaturesconfiguration_list_deviceconfigurationgroupassignment.md)|[deviceConfigurationGroupAssignment](../resources/intune_deviceconfig_deviceconfigurationgroupassignment.md) collection|Get the deviceConfigurationGroupAssignments from the groupAssignments navigation property.|
|[List deviceConfigurationDeviceStatuses](../api/intune_deviceconfig_macosdevicefeaturesconfiguration_list_deviceconfigurationdevicestatus.md)|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) collection|Get the deviceConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[List deviceConfigurationUserStatuses](../api/intune_deviceconfig_macosdevicefeaturesconfiguration_list_deviceconfigurationuserstatus.md)|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) collection|Get the deviceConfigurationUserStatuses from the userStatuses navigation property.|
|[Get deviceConfigurationDeviceOverview](../api/intune_deviceconfig_macosdevicefeaturesconfiguration_get_deviceconfigurationdeviceoverview.md)|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Get the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) from the deviceStatusOverview navigation property.|
|[Get deviceConfigurationUserOverview](../api/intune_deviceconfig_macosdevicefeaturesconfiguration_get_deviceconfigurationuseroverview.md)|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Get the [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) from the userStatusOverview navigation property.|

## Properties
|Property|Type|Description|
|---|---|---|
|id|String|Key of the entity. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|airPrintDestinations|[airPrintDestination](../resources/intune_deviceconfig_airprintdestination.md) collection|An array of AirPrint printers that should always be shown. Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune_deviceconfig_appledevicefeaturesconfigurationbase.md)|

## Relationships
|Relationship|Type|Description|
|---|---|---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune_deviceconfig_deviceconfigurationgroupassignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) collection|Device configuration installation stauts by device. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) collection|Device configuration installation stauts by user. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSDeviceFeaturesConfiguration"
}
-->
```json
{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "String",
      "resourcePath": "String"
    }
  ]
}
```



