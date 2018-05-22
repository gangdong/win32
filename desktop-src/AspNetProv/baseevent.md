﻿---
Description: 'The parent class from which all extrinsic ASP.NET event trace classes are derived.'
audience: developer
author: 'REDMOND\\markl'
manager: 'REDMOND\\markl'
ms.assetid: '581dc610-cb8d-417c-b7a6-3ce63010cc6e'
ms.prod: 'windows-server-dev'
ms.technology:
- 'asp.net'
- 'windows-management-instrumentation'
ms.tgt_platform: multiple
title: BaseEvent class
---

# BaseEvent class

The parent class from which all extrinsic ASP.NET event trace classes are derived.

The following syntax is simplified from Managed Object Format (MOF) code and includes all of the inherited properties.

## Syntax

``` syntax
[Dynamic, EventType(71), EventLevel(5), EventVersion(1), EventTypeName("BaseEvent")]
class BaseEvent : __ExtrinsicEvent
{
  uint8  SECURITY_DESCRIPTOR[];
  uint64 TIME_CREATED;
  string EventTime;
  string EventID;
  sint64 SequenceNumber;
  sint64 Occurrence;
  sint32 EventCode;
  sint32 EventDetailCode;
  string EventMessage;
  string ApplicationDomain;
  string TrustLevel;
  string ApplicationVirtualPath;
  string ApplicationPath;
  string MachineName;
  string CustomEventDetails;
  string SecurityDescriptor = "O:BAG:BAD:(A;;0x10000001;;;S-1-5-11)";
};
```

## Members

The **BaseEvent** class has these types of members:

-   [Properties](#properties)

### Properties

The **BaseEvent** class has these properties.

<dl> <dt>

**ApplicationDomain**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: **WmiDataId** (8), **StringTermination** ("NullTerminated"), **format** ("w")
</dt> </dl>

The application domain.

</dd> <dt>

**ApplicationPath**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: **WmiDataId** (11), **StringTermination** ("NullTerminated"), **format** ("w")
</dt> </dl>

The application path.

</dd> <dt>

**ApplicationVirtualPath**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: **WmiDataId** (10), **StringTermination** ("NullTerminated"), **format** ("w")
</dt> </dl>

The application virtual path.

</dd> <dt>

**CustomEventDetails**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: **WmiDataId** (13), **StringTermination** ("NullTerminated"), **format** ("w")
</dt> </dl>

Custom event details.

</dd> <dt>

**EventCode**
</dt> <dd> <dl> <dt>

Data type: **sint32**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: **WmiDataId** (5)
</dt> </dl>

The event code.

</dd> <dt>

**EventDetailCode**
</dt> <dd> <dl> <dt>

Data type: **sint32**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: **WmiDataId** (6)
</dt> </dl>

The event detail code.

</dd> <dt>

**EventID**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: **WmiDataId** (2), **StringTermination** ("NullTerminated"), **format** ("w")
</dt> </dl>

The identifier of the event.

</dd> <dt>

**EventMessage**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: **WmiDataId** (7), **StringTermination** ("NullTerminated"), **format** ("w")
</dt> </dl>

The message that describes the event.

</dd> <dt>

**EventTime**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: **WmiDataId** (1), **StringTermination** ("NullTerminated"), **format** ("w")
</dt> </dl>

The time the event occurred.

</dd> <dt>

**MachineName**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: **WmiDataId** (12), **StringTermination** ("NullTerminated"), **format** ("w")
</dt> </dl>

The name of the machine.

</dd> <dt>

**Occurrence**
</dt> <dd> <dl> <dt>

Data type: **sint64**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: **WmiDataId** (4)
</dt> </dl>

The *n*th occurrence of the event.

</dd> <dt>

**SECURITY\_DESCRIPTOR**
</dt> <dd> <dl> <dt>

Data type: **uint8** array
</dt> <dt>

Access type: Read-only
</dt> </dl>

Descriptor used by the event provider to determine which users can receive the event. This property is inherited from [**\_\_Event**](wmi.__event). For more information about constants used to set this security descriptor, see [WMI Security Constants](wmi.wmi_security_constants).

</dd> <dt>

**SecurityDescriptor**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Descriptor used by the event provider to determine which users can receive the event.

</dd> <dt>

**SequenceNumber**
</dt> <dd> <dl> <dt>

Data type: **sint64**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: **WmiDataId** (3)
</dt> </dl>

The event sequence number.

</dd> <dt>

**TIME\_CREATED**
</dt> <dd> <dl> <dt>

Data type: **uint64**
</dt> <dt>

Access type: Read-only
</dt> </dl>

Unique value that indicates the time at which the event was generated. This is a 64-bit value that represents the number of 100-nanosecond intervals after January 1, 1601. The information is in the Coordinated Universal Times (UTC) format. This property is inherited from [**\_\_Event**](wmi.__event).

For more information about using **uint64** values in scripts, see [Scripting in WMI](wmi.scripting_in_wmi).

</dd> <dt>

**TrustLevel**
</dt> <dd> <dl> <dt>

Data type: **string**
</dt> <dt>

Access type: Read-only
</dt> <dt>

Qualifiers: **WmiDataId** (9), **StringTermination** ("NullTerminated"), **format** ("w")
</dt> </dl>

The level of code access security (CAS) that is applied to the application.

</dd> </dl>

## Requirements



|                                     |                                                                                        |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista<br/>                                                               |
| Minimum supported server<br/> | Windows Server 2008<br/>                                                         |
| Namespace<br/>                | Root\\aspnet<br/>                                                                |
| MOF<br/>                      | <dl> <dt>AspNet.mof</dt> </dl>  |
| DLL<br/>                      | <dl> <dt>MSCoree.dll</dt> </dl> |



 

 



