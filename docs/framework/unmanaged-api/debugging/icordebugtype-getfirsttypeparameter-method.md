---
title: "ICorDebugType::GetFirstTypeParameter Method | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework-4.6"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-clr"
ms.tgt_pltfrm: ""
ms.topic: "reference"
apiname: 
  - "ICorDebugType.GetFirstTypeParameter"
apilocation: 
  - "mscordbi.dll"
apitype: "COM"
f1_keywords: 
  - "ICorDebugType::GetFirstTypeParameter"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "ICorDebugType::GetFirstTypeParameter method [.NET Framework debugging]"
  - "GetFirstTypeParameter method [.NET Framework debugging]"
ms.assetid: 35bb594f-af6a-4349-83fe-e98702674e03
caps.latest.revision: 11
author: "rpetrusha"
ms.author: "ronpet"
manager: "wpickett"
---
# ICorDebugType::GetFirstTypeParameter Method
Gets an interface pointer to an ICorDebugType that represents the first <xref:System.Type> parameter of the type represented by this `ICorDebugType`.  
  
## Syntax  
  
```  
HRESULT GetFirstTypeParameter (  
    [out] ICorDebugType   **value  
);  
```  
  
#### Parameters  
 `value`  
 [out] A pointer to the address of an `ICorDebugType` object that represents the first parameter.  
  
## Remarks  
 `GetFirstTypeParameter` can be called in cases where the additional information about the type involves, at most, one type parameter. In particular, it can be used if the type is an ELEMENT_TYPE_ARRAY, ELEMENT_TYPE_SZARRAY, ELEMENT_TYPE_BYREF, or ELEMENT_TYPE_PTR, as indicated by the [ICorDebugType::GetType](../../../../docs/framework/unmanaged-api/debugging/icordebugtype-gettype-method.md) method.  
  
## Requirements  
 **Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).  
  
 **Header:** CorDebug.idl, CorDebug.h  
  
 **Library:** CorGuids.lib  
  
 **.NET Framework Versions:** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]