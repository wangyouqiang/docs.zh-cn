---
title: ISymUnmanagedAsyncMethodPropertiesWriter::DefineKickoffMethod 方法
ms.date: 03/30/2017
ms.assetid: 4662f70d-817b-4374-8da8-e0545585939f
author: rpetrusha
ms.author: ronpet
ms.openlocfilehash: 38b4564aeb3c8ed4674e755e5691bb0a9d417bca
ms.sourcegitcommit: 6b308cf6d627d78ee36dbbae8972a310ac7fd6c8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "54624149"
---
# <a name="isymunmanagedasyncmethodpropertieswriterdefinekickoffmethod-method"></a>ISymUnmanagedAsyncMethodPropertiesWriter::DefineKickoffMethod 方法
设置启动异步操作的开始方法。  
  
## <a name="syntax"></a>语法  
  
```idl  
HRESULT DefineKickoffMethod(    [in] mdToken kickoffMethod);  
```  
  
#### <a name="parameters"></a>参数  
  
|参数|描述|  
|---------------|-----------------|  
|`kickoffMethod`||  
  
## <a name="return-value"></a>返回值  
 返回 `HRESULT`。  
  
## <a name="requirements"></a>要求  
 **标头：** CorSym.idl CorSym.h  
  
## <a name="see-also"></a>请参阅
- [ISymUnmanagedAsyncMethodPropertiesWriter 接口](../../../../docs/framework/unmanaged-api/diagnostics/isymunmanagedasyncmethodpropertieswriter-interface.md)
