---
title: "SetVirtualDirectory Method (WMI MSReportServer_ConfigurationSetting)"
description: "SetVirtualDirectory Method (WMI MSReportServer_ConfigurationSetting)"
author: maggiesMSFT
ms.author: maggies
ms.date: 03/01/2017
ms.service: reporting-services
ms.subservice: wmi-provider-library-reference
ms.topic: conceptual
ms.custom: updatefrequency5
helpviewer_keywords:
  - "SetVirtualDirectory method"
---
# ConfigurationSetting Method - SetVirtualDirectory
  Sets the name of the virtual directory for a given application.  
  
## Syntax  
  
```vb  
Public Sub SetVirtualDirectory(ByVal Application As String, _  
    ByVal VirtualDirectory As String, ByVal lcid As Int32, _  
    ByRef [Error] As String, ByRef HRESULT As Int32)  
```  
  
```csharp  
public void SetVirtualDirectory(string Application, string VirtualDirectory,   
       int Lcid,out string Error, out int HRESULT);  
```  
  
## Parameters  
 *Application*  
 The name of application for which to set the virtual directory.  
  
 *VirtualDirectory*  
 The name of the virtual directory.  
  
 *lcid*  
 The locale id for the virtual directory.  
  
 *Error*  
 [out] The description of the error that occurred.  
  
 *HRESULT*  
 [out] Value indicating whether the call succeeded or failed.  
  
## Return Value  
 Returns an *HRESULT* indicating success or failure of the method call. A value of 0 indicates that the method call was successful; an error code indicates the call was not successful.  
  
## Remarks  
 An application can have only one virtual directory name for all URL reservations.  
  
 VirtualDirectory must conform to naming conventions for virtual directories. VirtualDirectory must not be empty string or blank.  
  
 Updates the value of the \Configuration\URLReservations\Application\VirtualDirectory element. Succeeds even if no URL reservations have been created yet.  
  
## Requirements  
 **Namespace:** [!INCLUDE[ssRSWMInmspcA](../../includes/ssrswminmspca-md.md)]  
  
## See Also  
 [MSReportServer_ConfigurationSetting Members](../../reporting-services/wmi-provider-library-reference/msreportserver-configurationsetting-members.md)  
  
  
