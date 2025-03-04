---
UID: NF:comadmin.ICOMAdminCatalog2.GetApplicationInstanceIDFromProcessID
title: ICOMAdminCatalog2::GetApplicationInstanceIDFromProcessID (comadmin.h)
description: Retrieives the application instance identifier for the specified process identifier.
old-location: cos\icomadmincatalog2_getapplicationinstanceidfromprocessid.htm
tech.root: cossdk
ms.assetid: a09569af-11ec-406a-a51c-72b81b84fe41
ms.date: 12/05/2018
ms.keywords: GetApplicationInstanceIDFromProcessID, GetApplicationInstanceIDFromProcessID method [COM+], GetApplicationInstanceIDFromProcessID method [COM+],ICOMAdminCatalog2 interface, ICOMAdminCatalog2 interface [COM+],GetApplicationInstanceIDFromProcessID method, ICOMAdminCatalog2.GetApplicationInstanceIDFromProcessID, ICOMAdminCatalog2::GetApplicationInstanceIDFromProcessID, _cos_icomadmincatalog2_GetApplicationInstanceIDFromProcessID, comadmin/ICOMAdminCatalog2::GetApplicationInstanceIDFromProcessID, cos.icomadmincatalog2_getapplicationinstanceidfromprocessid
f1_keywords:
- comadmin/ICOMAdminCatalog2.GetApplicationInstanceIDFromProcessID
dev_langs:
- c++
req.header: comadmin.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: ComAdmin.Idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- ComAdmin.h
api_name:
- ICOMAdminCatalog2.GetApplicationInstanceIDFromProcessID
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ICOMAdminCatalog2::GetApplicationInstanceIDFromProcessID


## -description


Retrieives the application instance identifier for the specified process identifier.


## -parameters




### -param lProcessID [in]

The process ID.


### -param pbstrApplicationInstanceID [out, retval]

The corresponding application instance ID.


## -returns



This method can return the standard return values E_INVALIDARG, E_OUTOFMEMORY, E_UNEXPECTED, E_FAIL, and S_OK.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/comadmin/nn-comadmin-icomadmincatalog2">ICOMAdminCatalog2</a>
 

 

