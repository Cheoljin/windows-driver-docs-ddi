---
UID: NN:wudfddi.IFileCallbackCleanup
title: IFileCallbackCleanup
author: windows-driver-content
description: The framework can notify a driver when the driver should perform a cleanup operation.
old-location: wdf\ifilecallbackcleanup.htm
old-project: wdf
ms.assetid: d42eb7d5-6bf6-4f0f-a249-a869db486b6f
ms.author: windowsdriverdev
ms.date: 1/11/2018
ms.keywords: IWDFWorkItem, IWDFWorkItem::GetParentObject, GetParentObject
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: interface
req.header: wudfddi.h
req.include-header: Wudfddi.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.alt-api: IFileCallbackCleanup
req.alt-loc: Wudfddi.h
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: WUDFx.dll
req.irql: 
req.typenames: *PPOWER_ACTION, POWER_ACTION
req.product: Windows 10 or later.
---

# IFileCallbackCleanup interface



## -description
<p class="CCE_Message">[<b>Warning:</b> UMDF 2 is the latest version of UMDF and supersedes UMDF 1.  All new UMDF drivers should be written using UMDF 2.  No new features are being added to UMDF 1 and there is limited support for UMDF 1 on newer versions of Windows 10.  Universal Windows drivers must use UMDF 2.  For more info, see <a href="https://docs.microsoft.com/en-us/windows-hardware/drivers/wdf/getting-started-with-umdf-version-2">Getting Started with UMDF</a>.]

The framework can notify a driver when the driver should perform a cleanup operation.  The framework notifies the driver in response to an application calling the <b>CloseHandle</b> Microsoft Win32 function. The driver can handle the notification by registering the <b>IFileCallbackCleanup</b> interface.

A driver registers the <b>IFileCallbackCleanup</b> interface when it calls the <a href="https://msdn.microsoft.com/library/windows/hardware/ff558899">IWDFDriver::CreateDevice</a> method to create a device object. 



## -inheritance
The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IFileCallbackCleanup</b> interface inherits from the <a href="com.iunknown" xmlns:loc="http://microsoft.com/wdcml/l10n"><b>IUnknown</b></a> interface. <b>IFileCallbackCleanup</b> also has these types of members:

The <b>IFileCallbackCleanup</b> interface has these methods.

The <a href="https://msdn.microsoft.com/e6dd18f4-725f-4611-ad70-029654cf4375">OnCleanupFile</a> method cancels all I/O requests that a driver has pending in the framework queue. 

 


## -members
The <b>IFileCallbackCleanup</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://msdn.microsoft.com/library/windows/hardware/ff554905">IFileCallbackCleanup::OnCleanupFile</a>
</td>
<td align="left" width="63%">
The <a href="https://msdn.microsoft.com/e6dd18f4-725f-4611-ad70-029654cf4375">OnCleanupFile</a> method cancels all I/O requests that a driver has pending in the framework queue. 

</td>
</tr>
</table>The <a href="https://msdn.microsoft.com/e6dd18f4-725f-4611-ad70-029654cf4375">OnCleanupFile</a> method cancels all I/O requests that a driver has pending in the framework queue. 

 


## -remarks