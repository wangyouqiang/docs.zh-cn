---
title: 如何：转换图像颜色
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- bitmaps [Windows Forms], changing colors
- images [Windows Forms], changing colors
- image colors [Windows Forms]
ms.assetid: 2106fb9a-4d60-4dcf-9220-9f189a6c4d19
ms.openlocfilehash: 7a3ed1f3f6b3e89c8df160b7e753839e20acd877
ms.sourcegitcommit: 6b308cf6d627d78ee36dbbae8972a310ac7fd6c8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "54549754"
---
# <a name="how-to-translate-image-colors"></a>如何：转换图像颜色
翻译添加到一个或多个四个颜色组件值。 下表给出表示翻译颜色矩阵项。  
  
|要转换的组件|矩阵条目|  
|--------------------------------|------------------|  
|红色|[4][0]|  
|绿色|[4][1]|  
|蓝色|[4][2]|  
|Alpha|[4][3]|  
  
## <a name="example"></a>示例  
 下面的示例构造<xref:System.Drawing.Image>ColorBars.bmp 文件中的对象。 然后代码将添加到映像中的每个像素的红色组件的 0.75。 转换后的图像一起绘制原始图像。  
  
 下图显示在右侧左侧上的原始映像和转换后的图像。  
  
 ![转换颜色](../../../../docs/framework/winforms/advanced/media/colortrans2.png "colortrans2")  
  
 下表列出了四个条形的颜色矢量之前和之后的红色的转换。 请注意，因为颜色组件的最大值为 1，第二行中的红色组件不会更改。 （同样，颜色组件的最小值为 0。）  
  
|原始|目标语言|  
|--------------|----------------|  
|黑色 （0，0，0，1）|(0.75, 0, 0, 1)|  
|红色 （1，0，0，1）|(1, 0, 0, 1)|  
|绿色 （0、 1、 0、 1）|(0.75, 1, 0, 1)|  
|蓝色 （0，0，1，1）|(0.75, 0, 1, 1)|  
  
 [!code-csharp[System.Drawing.RecoloringImages#11](../../../../samples/snippets/csharp/VS_Snippets_Winforms/System.Drawing.RecoloringImages/CS/Class1.cs#11)]
 [!code-vb[System.Drawing.RecoloringImages#11](../../../../samples/snippets/visualbasic/VS_Snippets_Winforms/System.Drawing.RecoloringImages/VB/Class1.vb#11)]  
  
## <a name="compiling-the-code"></a>编译代码  
 前面的示例专用于 Windows 窗体，并且它需要<xref:System.Windows.Forms.PaintEventArgs> `e`，这是一个参数的<xref:System.Windows.Forms.Control.Paint>事件处理程序。 替换为`ColorBars.bmp`与图像文件名称和在您的系统都有效的路径。  
  
## <a name="see-also"></a>请参阅
- <xref:System.Drawing.Imaging.ColorMatrix>
- <xref:System.Drawing.Imaging.ImageAttributes>
- [Windows 窗体中的图形和绘制](../../../../docs/framework/winforms/advanced/graphics-and-drawing-in-windows-forms.md)
- [对图像重新着色](../../../../docs/framework/winforms/advanced/recoloring-images.md)
