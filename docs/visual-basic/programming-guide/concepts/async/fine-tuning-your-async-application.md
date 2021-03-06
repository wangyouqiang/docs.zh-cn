---
title: 微调异步应用程序 (Visual Basic)
ms.date: 07/20/2015
ms.assetid: 4c3e7997-a95f-4fbe-a6ac-60ba042d30b9
ms.openlocfilehash: 0dc03e1063b16c96916d4cac9214ddfa3333620b
ms.sourcegitcommit: 6b308cf6d627d78ee36dbbae8972a310ac7fd6c8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "54625150"
---
# <a name="fine-tuning-your-async-application-visual-basic"></a>微调异步应用程序 (Visual Basic)
可以使用由 <xref:System.Threading.Tasks.Task> 类型提供的方法和属性将精度和灵活性添加到异步应用程序。 本部分中的主题介绍使用 <xref:System.Threading.CancellationToken> 的示例和一些重要的 `Task` 方法，例如 <xref:System.Threading.Tasks.Task.WhenAll%2A?displayProperty=nameWithType> 和 <xref:System.Threading.Tasks.Task.WhenAny%2A?displayProperty=nameWithType>。  
  
 使用 `WhenAny` 和 `WhenAll` 可以更轻松地启动多个任务并通过监视单个任务待其完成。  
  
-   集合中的任何任务完成时，`WhenAny` 将返回完成的任务。  
  
     有关示例，请使用`WhenAny`，请参阅[一个是完整 (Visual Basic 中) 后取消剩余异步任务](../../../../visual-basic/programming-guide/concepts/async/cancel-remaining-async-tasks-after-one-is-complete.md)并[启动多个异步任务和过程其完成时进行 (Visual Basic)](../../../../visual-basic/programming-guide/concepts/async/start-multiple-async-tasks-and-process-them-as-they-complete.md)。  
  
-   集合中的所有任务完成时，`WhenAll` 将返回完成的任务。  
  
     有关详细信息和使用的示例， `WhenAll`，请参阅[如何：使用 (Visual Basic) Task.WhenAll 扩展异步演练](../../../../visual-basic/programming-guide/concepts/async/how-to-extend-the-async-walkthrough-by-using-task-whenall.md)。  
  
 本部分包括下列示例。  
  
-   [取消一个异步任务或一组任务 (Visual Basic)](../../../../visual-basic/programming-guide/concepts/async/cancel-an-async-task-or-a-list-of-tasks.md)。  
  
-   [时间 (Visual Basic 中) 的一段时间后取消异步任务](../../../../visual-basic/programming-guide/concepts/async/cancel-async-tasks-after-a-period-of-time.md)  
  
-   [后取消剩余异步任务之一完成 (Visual Basic)](../../../../visual-basic/programming-guide/concepts/async/cancel-remaining-async-tasks-after-one-is-complete.md)  
  
-   [启动多个异步任务并在它们完成 (Visual Basic 中) 时进行处理](../../../../visual-basic/programming-guide/concepts/async/start-multiple-async-tasks-and-process-them-as-they-complete.md)  
  
> [!NOTE]
>  若要运行该示例，计算机上必须安装有 Visual Studio 2012 或更高版本和 .NET Framework 4.5 或更高版本。  
  
 项目将创建一个 UI，其中包含用于启动进程和取消进程的按钮，如下图所示。 这些按钮名为 `startButton` 和 `cancelButton`。  
  
 ![WPF 窗口与“取消”按钮](../../../../csharp/programming-guide/concepts/async/media/cancellation.png "取消")  
  
 您可以下载完整的 Windows Presentation Foundation (WPF) 项目，从[异步示例：你的应用程序进行微调](https://code.msdn.microsoft.com/Async-Fine-Tuning-Your-a676abea)。  
  
## <a name="see-also"></a>请参阅
- [使用 Async 和 Await 的异步编程 (Visual Basic)](../../../../visual-basic/programming-guide/concepts/async/index.md)
