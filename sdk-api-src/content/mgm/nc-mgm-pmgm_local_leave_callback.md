---
UID: NC:mgm.PMGM_LOCAL_LEAVE_CALLBACK
title: PMGM_LOCAL_LEAVE_CALLBACK (mgm.h)
description: The PMGM_LOCAL_LEAVE_CALLBACK callback is a call into a routing protocol to notify the routing protocol that the IGMP has detected that it no longer has receivers for a group on an interface that is currently owned by the routing protocol.
old-location: rras\pmgm_local_leave_callback.htm
tech.root: RRAS
ms.assetid: 9569c0e5-f9bb-4dc9-9689-f97d107697b5
ms.date: 12/05/2018
ms.keywords: MgmLocalLeaveCallback, PMGM_LOCAL_LEAVE_CALLBACK, PMGM_LOCAL_LEAVE_CALLBACK callback, PMGM_LOCAL_LEAVE_CALLBACK callback function [RAS], _mpr_pmgm_local_leave_callback, mgm/PMGM_LOCAL_LEAVE_CALLBACK, rras.pmgm_local_leave_callback
f1_keywords:
- mgm/PMGM_LOCAL_LEAVE_CALLBACK
dev_langs:
- c++
req.header: mgm.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: None supported
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
- UserDefined
api_location:
- Mgm.h
api_name:
- PMGM_LOCAL_LEAVE_CALLBACK
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# PMGM_LOCAL_LEAVE_CALLBACK callback function


## -description


The 
<b>PMGM_LOCAL_LEAVE_CALLBACK</b> callback is a call into a routing protocol to notify the routing protocol that the IGMP has detected that it no longer has receivers for a group on an interface that is currently owned by the routing protocol.

This callback is invoked when the 
<a href="https://docs.microsoft.com/windows/desktop/api/mgm/nf-mgm-mgmdeletegroupmembershipentry">MgmDeleteGroupMembershipEntry</a> function is called by IGMP.


## -parameters




### -param dwSourceAddr [in]

Specifies the source address from which to stop receiving multicast data. Zero indicates to stop receiving data from all sources (a wildcard receiver for a group); otherwise, the value of <i>dwSourceAddr</i> is the IP address of the source or source network. 




To specify a range of source addresses, the multicast group manager specifies the source network using <i>dwSourceAddr</i>, and specifies a subnet mask using <i>dwSourceMask</i>.


### -param dwSourceMask [in]

Specifies the subnet mask that corresponds to <i>dwSourceAddr</i>. The <i>dwSourceAddr</i> and <i>dwSourceMask</i> parameters are used together to define a range of sources from which to stop receiving multicast data. 




The multicast group manager specifies zero for this parameter if it also specified zero for <i>dwSourceAddr</i> (a wildcard receiver).
						


### -param dwGroupAddr [in]

Specifies the multicast group for which to stop receiving data. Zero indicates to stop receiving data for all groups (a wildcard receiver); otherwise, the value of <i>dwGroupAddr</i> is the IP address of the group. 




To specify a range of group addresses, the multicast group manager specifies the group address using <i>dwGroupAddr</i>, and specifies a subnet mask using <i>dwGroupMask</i>.


### -param dwGroupMask [in]

Specifies the subnet mask that corresponds to <i>dwGroupAddr</i>. The <i>dwGroupAddr</i> and <i>dwGroupMask</i> parameters are used together to define a range of multicast groups. 




The multicast group manager specifies zero for this parameter if it also specified zero for <i>dwGroupAddr</i> (a wildcard receiver).


### -param dwIfIndex [in]

Specifies the interface on which to stop receiving multicast data.


### -param dwIfNextHopAddr [in]

Specifies the address of the next hop that corresponds to the index specified by <i>dwIfIndex</i>. The <i>dwIfIndex</i> and <i>dwIfNextHopIPAddr</i> parameters uniquely identify a next hop on point-to-multipoint interfaces. A point-to-multipoint interface is a connection where one interface connects to multiple networks. Examples of point-to-multipoint interfaces include non-broadcast multiple access (NBMA) interfaces and the internal interface on which all dial-up clients connect. 




For broadcast interfaces (such as Ethernet interfaces) or point-to-point interfaces, which are identified by only the value of <i>dwIfIndex</i>, specify zero.


## -returns



RRAS does not expect the application to return any specific value; any value returned is ignored by RRAS.




## -remarks



This version of the Multicast Group Manager API supports only wildcard sources (*, g) or specific sources (s, g), not a range of sources. The same restriction applies to groups (that is, no group ranges are permitted).




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/mgm/nc-mgm-pmgm_local_join_callback">PMGM_LOCAL_JOIN_CALLBACK</a>
 

 

