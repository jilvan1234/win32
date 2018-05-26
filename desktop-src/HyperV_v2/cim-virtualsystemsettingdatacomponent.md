---
Description: Represents a portion of a relationship between a CIM\_VirtualSystemSettingData instance and a set of CIM\_ResourceAllocationSettingData instances.
ms.assetid: 4f167517-079e-4b5f-885a-741ac1d1dc71
title: CIM\_VirtualSystemSettingDataComponent class
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# CIM\_VirtualSystemSettingDataComponent class

Represents a portion of a relationship between a [**CIM\_VirtualSystemSettingData**](cim-virtualsystemsettingdata.md) instance and a set of [**CIM\_ResourceAllocationSettingData**](cim-resourceallocationsettingdata.md) instances.

## Syntax

``` syntax
[Association, Aggregation, Abstract, Version("2.22.0"), UMLPackagePath("CIM::System::SystemElements"), AMENDMENT]
class CIM_VirtualSystemSettingDataComponent : CIM_Component
{
  CIM_VirtualSystemSettingData      REF GroupComponent;
  CIM_ResourceAllocationSettingData REF PartComponent;
};
```

## Members

The **CIM\_VirtualSystemSettingDataComponent** class has these types of members:

-   [Properties](#properties)

### Properties

The **CIM\_VirtualSystemSettingDataComponent** class has these properties.

<dl> <dt>

**GroupComponent**
</dt> <dd> <dl> <dt>

Data type: **CIM\_VirtualSystemSettingData**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Aggregate**](https://msdn.microsoft.com/library/aa393650), [**Override**](https://msdn.microsoft.com/library/aa393650) ("GroupComponent")
</dt> </dl>

A reference to the top-level [**CIM\_VirtualSystemSettingData**](cim-virtualsystemsettingdata.md) object of the virtual system configuration.

</dd> <dt>

**PartComponent**
</dt> <dd> <dl> <dt>

Data type: **CIM\_ResourceAllocationSettingData**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: [**Override**](https://msdn.microsoft.com/library/aa393650) ("PartComponent")
</dt> </dl>

A reference the [**CIM\_ResourceAllocationSettingData**](cim-resourceallocationsettingdata.md) object that represents a part of the virtual system configuration.

</dd> </dl>

## Requirements



|                                     |                                                                                                         |
|-------------------------------------|---------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 8<br/>                                                                                    |
| Minimum supported server<br/> | Windows Server 2012<br/>                                                                          |
| Namespace<br/>                | Root\\virtualization\\v2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>WindowsVirtualization.V2.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Vmms.exe</dt> </dl>                     |



## See also

<dl> <dt>

[**CIM\_Component**](cim-component.md)
</dt> </dl>

 

 



