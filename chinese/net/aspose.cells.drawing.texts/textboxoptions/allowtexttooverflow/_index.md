---
title: "TextBoxOptions.AllowTextToOverflow"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TextBoxOptions 属性。是否允许文本溢出形状"
type: docs
url: /zh/net/aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/
---
## TextBoxOptions.AllowTextToOverflow property

是否允许文本溢出形状。

```csharp
public bool AllowTextToOverflow { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyAllowTextToOverflowDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加文本框
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // 设置可能会溢出的文本
            textBox.Text = "This is a long text that might overflow the text box boundaries if AllowTextToOverflow is false";

            // 启用文本溢出
            textBox.TextBoxOptions.AllowTextToOverflow = true;

            // 保存工作簿
            workbook.Save("TextBoxAllowTextToOverflowDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


