---
UID: NE:ntdddisk._DETECTION_TYPE
title: "_DETECTION_TYPE"
description: The DETECTION_TYPE enumeration type is used in conjunction with the IOCTL_DISK_GET_DRIVE_GEOMETRY_EX request and the DISK_GEOMETRY_EX structure to determine the type of formatting used by the BIOS to record the disk geometry.
old-location: storage\detection_type.htm
tech.root: storage
ms.assetid: 3257a207-dd7e-4321-b037-95d62cea6f76
ms.date: 03/29/2018
ms.keywords: DETECTION_TYPE, DETECTION_TYPE enumeration [Storage Devices], DetectExInt13, DetectInt13, DetectNone, _DETECTION_TYPE, ntdddisk/DETECTION_TYPE, ntdddisk/DetectExInt13, ntdddisk/DetectInt13, ntdddisk/DetectNone, storage.detection_type, structs-disk_2d3d7a57-abcd-43b2-a62d-8b8c45a9fca0.xml
ms.topic: enum
req.header: ntdddisk.h
req.include-header: Ntdddisk.h, Ntddk.h, Ntdddisk.h
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
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	ntdddisk.h
api_name:
-	DETECTION_TYPE
product:
- Windows
targetos: Windows
req.typenames: DETECTION_TYPE
---

# _DETECTION_TYPE enumeration


## -description


The DETECTION_TYPE enumeration type is used in conjunction with the <a href="https://msdn.microsoft.com/library/windows/hardware/ff560359">IOCTL_DISK_GET_DRIVE_GEOMETRY_EX</a> request and the <a href="https://msdn.microsoft.com/library/windows/hardware/ff552618">DISK_GEOMETRY_EX</a> structure to determine the type of formatting used by the BIOS to record the disk geometry. 


## -enum-fields




### -field DetectNone

Indicates that the disk contains neither an INT 13h partition nor an extended INT 13h partition.


### -field DetectInt13

Indicates that the disk has a standard INT 13h partition.


### -field DetectExInt13

Indicates that the disk contains an extended INT 13h partition. 


## -remarks



Possible formatting types are the standard INT 13h partition format or the extended INT 13h partition format. 




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff552601">DISK_DETECTION_INFO</a>
 

 

