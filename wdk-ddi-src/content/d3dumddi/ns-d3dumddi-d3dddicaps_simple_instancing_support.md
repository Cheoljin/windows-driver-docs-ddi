---
UID: NS:d3dumddi.D3DDDICAPS_SIMPLE_INSTANCING_SUPPORT
title: D3DDDICAPS_SIMPLE_INSTANCING_SUPPORT
description: Describes whether simple instancing is supported.
old-location: display\d3dddicaps_simple_instancing_support.htm
tech.root: display
ms.assetid: CF75EBC8-D756-49B5-BC1F-1DBE8DC04137
ms.date: 05/10/2018
ms.keywords: D3DDDICAPS_SIMPLE_INSTANCING_SUPPORT, D3DDDICAPS_SIMPLE_INSTANCING_SUPPORT structure [Display Devices], d3dumddi/D3DDDICAPS_SIMPLE_INSTANCING_SUPPORT, display.d3dddicaps_simple_instancing_support
ms.topic: struct
req.header: d3dumddi.h
req.include-header: D3d10umddi.h
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1
req.target-min-winversvr: Windows Server 2012 R2
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
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	D3dumddi.h
api_name:
-	D3DDDICAPS_SIMPLE_INSTANCING_SUPPORT
product:
- Windows
targetos: Windows
req.typenames: D3DDDICAPS_SIMPLE_INSTANCING_SUPPORT
---

# D3DDDICAPS_SIMPLE_INSTANCING_SUPPORT structure


## -description


Describes whether simple instancing is supported.


## -struct-fields




### -field SimpleInstancingSupported

Specifies whether the hardware and the user-mode driver support simple instancing. The Direct3D runtime sets this member to <b>TRUE</b> if the hardware and driver support simple instancing and the driver is a Direct3D Level 9 driver and supports Windows Display Driver Model (WDDM) 1.3 and later. Otherwise this member is <b>FALSE</b>.

Used only by Direct3D Level 9 drivers that support WDDM 1.3 and later.

Supported starting with Windows 8.1.


## -remarks



Instancing capabilities are exposed through the <b>D3DDDICAPS_GET_SIMPLE_INSTANCING_SUPPORT</b> constant value of the <a href="https://msdn.microsoft.com/library/windows/hardware/ff544132">D3DDDICAPS_TYPE</a> enumeration.

For more info on simple instancing, see The Microsoft Direct3D 11 topic, <a href="https://msdn.microsoft.com/940381BB-E8F6-416D-8F36-CC3591E70703">D3D11_FEATURE_DATA_D3D9_SIMPLE_INSTANCING_SUPPORT</a>.




## -see-also




<a href="https://msdn.microsoft.com/940381BB-E8F6-416D-8F36-CC3591E70703">D3D11_FEATURE_DATA_D3D9_SIMPLE_INSTANCING_SUPPORT</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff544132">D3DDDICAPS_TYPE</a>
 

 

