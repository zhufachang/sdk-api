---
UID: NS:wininet.__unnamed_struct_5
title: INTERNET_PER_CONN_OPTION_LISTA (wininet.h)
description: Contains the list of options for a particular Internet connection.
old-location: wininet\internet_per_conn_option_list.htm
tech.root: wininet
ms.assetid: 5e3178d5-b266-44bd-846c-f14bad0083c4
ms.date: 12/05/2018
ms.keywords: '*LPINTERNET_PER_CONN_OPTION_LISTA, INTERNET_PER_CONN_OPTION_LIST, INTERNET_PER_CONN_OPTION_LIST structure [WinINet], INTERNET_PER_CONN_OPTION_LISTA, INTERNET_PER_CONN_OPTION_LISTW, LPINTERNET_PER_CONN_OPTION_LIST, LPINTERNET_PER_CONN_OPTION_LIST structure pointer [WinINet], _inet_internet_per_conn_option_list_structure, wininet.internet_per_conn_option_list, wininet/INTERNET_PER_CONN_OPTION_LIST, wininet/INTERNET_PER_CONN_OPTION_LISTA, wininet/INTERNET_PER_CONN_OPTION_LISTW, wininet/LPINTERNET_PER_CONN_OPTION_LIST'
f1_keywords:
- wininet/INTERNET_PER_CONN_OPTION_LIST
dev_langs:
- c++
req.header: wininet.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: INTERNET_PER_CONN_OPTION_LISTW (Unicode) and INTERNET_PER_CONN_OPTION_LISTA (ANSI)
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
- Wininet.h
api_name:
- INTERNET_PER_CONN_OPTION_LIST
- INTERNET_PER_CONN_OPTION_LISTA
- INTERNET_PER_CONN_OPTION_LISTW
targetos: Windows
req.typenames: INTERNET_PER_CONN_OPTION_LISTA, *LPINTERNET_PER_CONN_OPTION_LISTA
req.redist: 
ms.custom: 19H1
---

# INTERNET_PER_CONN_OPTION_LISTA structure


## -description


Contains the list of options for a particular Internet connection.


## -struct-fields




### -field dwSize

Size of the 
structure, in bytes.


### -field pszConnection

Pointer to a string that contains the name of the RAS connection or <b>NULL</b>, which indicates the default or LAN connection, to set or query options on. 


### -field dwOptionCount

Number of options to query or set. 


### -field dwOptionError

Options that failed, if an error occurs. 


### -field pOptions

Pointer to an array of 
<a href="https://docs.microsoft.com/windows/desktop/api/wininet/ns-wininet-internet_per_conn_optiona">INTERNET_PER_CONN_OPTION</a> structures containing the options to query or set. 


## -remarks



In Microsoft Internet Explorer 5, only the ANSI versions of 
<a href="https://docs.microsoft.com/windows/desktop/api/wininet/nf-wininet-internetqueryoptiona">InternetQueryOption</a> and 
<a href="https://docs.microsoft.com/windows/desktop/api/wininet/nf-wininet-internetsetoptiona">InternetSetOption</a> will work with the 
<b>INTERNET_PER_CONN_OPTION_LIST</b> structure. The Unicode versions will support using the 
<b>INTERNET_PER_CONN_OPTION_LIST</b> structure in later versions of Internet Explorer.

<div class="alert"><b>Note</b>  WinINet does not support server implementations. In addition, it should not be used from a service.  For server implementations or services use <a href="https://docs.microsoft.com/windows/desktop/WinHttp/winhttp-start-page">Microsoft Windows HTTP Services (WinHTTP)</a>.</div>
<div> </div>



## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/wininet/ns-wininet-internet_per_conn_optiona">INTERNET_PER_CONN_OPTION</a>



<a href="https://docs.microsoft.com/windows/desktop/api/wininet/nf-wininet-internetqueryoptiona">InternetQueryOption</a>



<a href="https://docs.microsoft.com/windows/desktop/api/wininet/nf-wininet-internetsetoptiona">InternetSetOption</a>
 

 

