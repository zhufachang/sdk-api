---
UID: NF:http.HTTPAPI_EQUAL_VERSION
title: HTTPAPI_EQUAL_VERSION macro (http.h)
description: Returns a non-zero value if an HTTPAPI_VERSION structure is exactly equal to a specified major/minor version combination, or zero otherwise.
old-location: http\httpapi_equal_version.htm
tech.root: http
ms.assetid: e6af7b3a-2e2f-4a50-bef6-9e5b6503cd71
ms.date: 12/05/2018
ms.keywords: HTTPAPI_EQUAL_VERSION, HTTPAPI_EQUAL_VERSION macro [HTTP], http.httpapi_equal_version, http/HTTPAPI_EQUAL_VERSION
f1_keywords:
- http/HTTP_EQUAL_VERSION
dev_langs:
- c++
req.header: http.h
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
- http.h
api_name:
- HTTP_EQUAL_VERSION
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# HTTPAPI_EQUAL_VERSION macro


## -description


The <b>HTTPAPI_EQUAL_VERSION</b>returns a non-zero value if an 
<a href="https://docs.microsoft.com/windows/desktop/api/http/ns-http-httpapi_version">HTTPAPI_VERSION</a> structure is exactly equal to a specified major/minor version combination, or zero otherwise.


## -parameters




### -param version

The 
<a href="https://docs.microsoft.com/windows/desktop/api/http/ns-http-httpapi_version">HTTPAPI_VERSION</a> structure to be examined.


### -param major

The major portion of the version to be compared.


### -param minor

The minor portion of the version to be compared.


## -see-also




<a href="https://docs.microsoft.com/windows/desktop/Http/http-server-api-version-1-0-macros">HTTP Server API Version 1.0 Macros</a>
 

 

