---
UID: NS:oaidl.tagBINDPTR
title: BINDPTR (oaidl.h)
description: Describes a pointer.
old-location: automat\bindptr.htm
tech.root: automat
ms.assetid: 7035df31-3b13-4297-8464-b86f64d38f20
ms.date: 12/05/2018
ms.keywords: '*LPBINDPTR, BINDPTR, BINDPTR structure [Automation], LPBINDPTR, LPBINDPTR structure pointer [Automation], _oa96_BINDPTR, automat.bindptr, oaidl/BINDPTR, oaidl/LPBINDPTR'
f1_keywords:
- oaidl/BINDPTR
dev_langs:
- c++
req.header: oaidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
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
- HeaderDef
api_location:
- OaIdl.h
api_name:
- BINDPTR
targetos: Windows
req.typenames: BINDPTR, *LPBINDPTR
req.redist: 
ms.custom: 19H1
---

# BINDPTR structure


## -description


Describes a pointer.


## -struct-fields




### -field lpfuncdesc

Pointer to a function.


### -field lpvardesc

Pointer to a variable, constant, or data member.


### -field lptcomp

The <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/oaidl/nn-oaidl-itypecomp">ITypeComp</a> that binds the pointer.

