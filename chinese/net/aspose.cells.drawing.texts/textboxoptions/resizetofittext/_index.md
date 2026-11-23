---
title: "TextBoxOptions.ResizeToFitText"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TextBoxOptions 属性。指示是否将形状大小调整以适应文本"
type: docs
url: /zh/net/aspose.cells.drawing.texts/textboxoptions/resizetofittext/
---
## TextBoxOptions.ResizeToFitText property

指示是否调整形状大小以适应文本

```csharp
public bool ResizeToFitText { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyResizeToFitTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建一个具有正确参数的文本框
            Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(1, 1, 100, 100, 200, 50);
            textBox.Text = "This is a sample text that will make the text box resize to fit";

            // 正确访问 TextBoxOptions
            textBox.TextBoxOptions.ResizeToFitText = true;

            // 保存工作簿
            workbook.Save("TextBoxResizeToFitTextDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


