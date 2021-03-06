---
title: 如何：绘制具有线帽的线条
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- drawing [Windows Forms], lines
- lines [Windows Forms], drawing
- pens [Windows Forms], drawing lines
- drawing lines [Windows Forms], line caps
ms.assetid: eb68c3e1-c400-4886-8a04-76978a429cb6
ms.openlocfilehash: a0d4d92d7201c4ac09eadd11d8f2e38a3c80c287
ms.sourcegitcommit: 6b308cf6d627d78ee36dbbae8972a310ac7fd6c8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "54713126"
---
# <a name="how-to-draw-a-line-with-line-caps"></a>如何：绘制具有线帽的线条
可以在一个名为线帽的多个形状绘制的开始或结束的行。 [!INCLUDE[ndptecgdiplus](../../../../includes/ndptecgdiplus-md.md)] 支持多种线帽，如 round、 正方形、 菱形和箭头。  
  
## <a name="example"></a>示例  
 您可以指定行 （起始端），行 （末端） 的末尾或虚线 (dash cap) 的短划线开头的线帽。  
  
 下面的示例绘制一个行，其中一端箭头和另一端圆端帽。 该图显示了最终得到的行：  
  
 ![笔](../../../../docs/framework/winforms/advanced/media/pens4.gif "pens4")  
  
 [!code-csharp[System.Drawing.UsingAPen#71](../../../../samples/snippets/csharp/VS_Snippets_Winforms/System.Drawing.UsingAPen/CS/Class1.cs#71)]
 [!code-vb[System.Drawing.UsingAPen#71](../../../../samples/snippets/visualbasic/VS_Snippets_Winforms/System.Drawing.UsingAPen/VB/Class1.vb#71)]  
  
## <a name="compiling-the-code"></a>编译代码  
  
-   创建 Windows 窗体和处理该窗体<xref:System.Windows.Forms.Control.Paint>事件。 示例将代码粘贴到<xref:System.Windows.Forms.Control.Paint>事件处理程序传递`e`作为<xref:System.Windows.Forms.PaintEventArgs>。  
  
## <a name="see-also"></a>请参阅
- <xref:System.Drawing.Pen?displayProperty=nameWithType>
- <xref:System.Drawing.Drawing2D.LineCap?displayProperty=nameWithType>
- [Windows 窗体中的图形和绘制](../../../../docs/framework/winforms/advanced/graphics-and-drawing-in-windows-forms.md)
- [使用笔绘制直线和形状](../../../../docs/framework/winforms/advanced/using-a-pen-to-draw-lines-and-shapes.md)
