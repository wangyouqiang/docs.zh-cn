---
title: 如何：执行返回嵌套的集合的查询
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
ms.assetid: f7f385f3-ffcf-4f3b-af35-de8818938e5f
ms.openlocfilehash: f429b8e8f546669fba64b9ee04222d399971936e
ms.sourcegitcommit: 6b308cf6d627d78ee36dbbae8972a310ac7fd6c8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "54654511"
---
# <a name="how-to-execute-a-query-that-returns-nested-collections"></a>如何：执行返回嵌套的集合的查询
这些内容演示如何使用 <xref:System.Data.EntityClient.EntityCommand> 对象针对概念模型执行命令，以及如何使用 <xref:System.Data.EntityClient.EntityDataReader> 检索嵌套集合结果。  
  
### <a name="to-run-the-code-in-this-example"></a>运行本示例中的代码  
  
1.  添加[AdventureWorks 销售模型](https://msdn.microsoft.com/library/f16cd988-673f-4376-b034-129ca93c7832)到你的项目和配置项目以使用[!INCLUDE[adonet_ef](../../../../../includes/adonet-ef-md.md)]。 有关详细信息，请参阅[如何：使用实体数据模型向导](https://msdn.microsoft.com/library/dadb058a-c5d9-4c5c-8b01-28044112231d)。  
  
2.  在应用程序的代码页中，添加以下 `using` 语句（在 Visual Basic 中为 `Imports`）：  
  
     [!code-csharp[DP EntityServices Concepts#Namespaces](../../../../../samples/snippets/csharp/VS_Snippets_Data/dp entityservices concepts/cs/source.cs#namespaces)]
     [!code-vb[DP EntityServices Concepts#Namespaces](../../../../../samples/snippets/visualbasic/VS_Snippets_Data/dp entityservices concepts/vb/source.vb#namespaces)]  
  
## <a name="example"></a>示例  
 一个*嵌套集合*是位于另一个集合的集合。 以下代码检索 `Contacts` 的集合以及与每个 `SalesOrderHeaders` 关联的 `Contact` 的嵌套集合。  
  
 [!code-csharp[DP EntityServices Concepts#ReturnNestedCollectionWithEntityCommand](../../../../../samples/snippets/csharp/VS_Snippets_Data/dp entityservices concepts/cs/source.cs#returnnestedcollectionwithentitycommand)]
 [!code-vb[DP EntityServices Concepts#ReturnNestedCollectionWithEntityCommand](../../../../../samples/snippets/visualbasic/VS_Snippets_Data/dp entityservices concepts/vb/source.vb#returnnestedcollectionwithentitycommand)]  
  
## <a name="see-also"></a>请参阅
- [用于实体框架的 EntityClient 提供程序](../../../../../docs/framework/data/adonet/ef/entityclient-provider-for-the-entity-framework.md)
