---
title: SqlStreamChars.Seek （Int64，SeekOrigin） 方法 (System.Data.SqlTypes)
author: douglaslMS
ms.author: douglasl
ms.date: 12/20/2018
ms.technology:
- dotnet-data
topic_type:
- apiref
api_name:
- System.Data.SqlTypes.SqlStreamChars.Seek
api_location:
- System.Data.dll
api_type:
- Assembly
ms.openlocfilehash: 1710c802324920e324b18ddea843f0a532fa0d17
ms.sourcegitcommit: a36cfc9dbbfc04bd88971f96e8a3f8e283c15d42
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "54222982"
---
# <a name="sqlstreamcharsseekint64-seekorigin-method"></a>SqlStreamChars.Seek （Int64，SeekOrigin） 方法

当在派生类中重写时，设置当前流中的位置。 包含此方法的程序集具有与 SQLAccess.dll 友元关系。 它被用于 SQL server 上。 对于其他数据库，使用提供该数据库的宿主机制。

```csharp
public abstract long Seek (long offset, System.IO.SeekOrigin origin);
```

## <a name="parameters"></a>参数

`offset`\
字节偏移量相对于`origin`。

`origin`\
一个枚举值，该值指示要从中获取新位置的参考点。

## <a name="returns"></a>返回

<xref:System.Int32>\
当前流中的新位置。

## <a name="remarks"></a>备注

> [!WARNING]
> `SqlStreamChars.Seek`方法是私有的不适合直接在代码中使用。
>
> Microsoft 不支持在生产应用程序在任何情况下使用此字段。

## <a name="requirements"></a>要求

**Namespace**：<xref:System.Data.SqlTypes>

**程序集：** System.Data （在 System.Data.dll 中)

**.NET framework 版本：** 自 2.0 之后可用。