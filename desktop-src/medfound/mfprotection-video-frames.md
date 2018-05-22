﻿---
Description: 'Specifies if an application is allowed access to uncompressed video frames.'
ms.assetid: '7D2A9003-B36E-4082-877E-8AC7F5645E89'
title: 'MFPROTECTION\_VIDEO\_FRAMES attribute'
---

# MFPROTECTION\_VIDEO\_FRAMES attribute

Specifies if an application is allowed access to uncompressed video frames.

## Data type

**UINT32**

## Remarks

A value of 0 indicates that the application is allowed access to the frames. This might be determined as a result of a private agreement between the application and the particular content protection system in use.

A value of 1 indicates that the application is allowed access to frames if a valid application certificate is provided by the application (see [**IMFMediaEngineProtectedContent::SetApplicationCertificate**](imfmediaengineprotectedcontent-setapplicationcertificate.md)).

A value of 0xFFFFFFFF, which is the default value, indicates no applications are allowed access to uncompressed frames.

## Requirements



|                                     |                                                                                    |
|-------------------------------------|------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 8 \[UWP apps only\]<br/>                                             |
| Minimum supported server<br/> | Windows Server 2012 \[UWP apps only\]<br/>                                   |
| Header<br/>                   | <dl> <dt>Mfidl.h</dt> </dl> |



## See also

<dl> <dt>

[Alphabetical List of Media Foundation Attributes](alphabetical-list-of-media-foundation-attributes.md)
</dt> <dt>

[Media Type Attributes](media-type-attributes.md)
</dt> </dl>

 

 



