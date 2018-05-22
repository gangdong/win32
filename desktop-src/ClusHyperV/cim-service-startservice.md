---
title: StartService method of the CIM\_Service class
description: Starts the service.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: '26c15882-a7fb-48d6-80f3-c6a00efb5f1e'
ms.prod: 'windows-server-dev'
ms.technology:
- 'failover-cluster-hyperv'
- 'windows-management-instrumentation'
ms.tgt_platform: multiple
keywords: ["StartService method", "StartService method, CIM_Service class", "CIM_Service class, StartService method"]
topic_type:
- apiref
api_name:
- CIM_Service.StartService
api_location:
- VMMS.exe
api_type:
- COM
---

# StartService method of the CIM\_Service class

Starts the service.

The [**StartService**](https://msdn.microsoft.com/library/aa393655) method puts the service in a started state.

## Syntax


```mof
uint32 StartService();
```



## Parameters

This method has no parameters.

## Return value

Returns "0" on success, otherwise returns a WMI error code.

## Requirements



|                                     |                                                                                                        |
|-------------------------------------|--------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                              |
| Minimum supported server<br/> | Windows Server�2016<br/>                                                                         |
| Namespace<br/>                | Root\\HyperVCluster\\v2<br/>                                                                     |
| MOF<br/>                      | <dl> <dt>WindowsHyperVCluster.V2.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>VMMS.exe</dt> </dl>                    |



## See also

<dl> <dt>

[**CIM\_Service**](cim-service.md)
</dt> </dl>

�

�




