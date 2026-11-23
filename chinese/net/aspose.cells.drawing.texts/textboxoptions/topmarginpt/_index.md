---
title: "TextBoxOptions.TopMarginPt"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TextBoxOptions 属性。获取并设置以点为单位的上边距"
type: docs
url: /zh/net/aspose.cells.drawing.texts/textboxoptions/topmarginpt/
---
## TextBoxOptions.TopMarginPt property

获取和设置以点为单位的顶部边距。

```csharp
public double TopMarginPt { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyTopMarginPtDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 向工作表添加文本框
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            
            // 以点设置上边距
            textBox.TextBoxOptions.TopMarginPt = 0.2d;
            
            // 保存工作簿
            workbook.Save("TextBoxTopMarginDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


