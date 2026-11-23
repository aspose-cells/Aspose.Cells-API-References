---
title: "TextBoxOptions.ShapeTextVerticalAlignment"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TextBoxOptions 属性。它对应于 Excel 中的 Format Shape  Text Options  Text Box  Vertical Alignment。"
type: docs
url: /zh/net/aspose.cells.drawing.texts/textboxoptions/shapetextverticalalignment/
---
## TextBoxOptions.ShapeTextVerticalAlignment property

它对应 Excel 中的“格式形状 - 文本选项 - 文本框 - 垂直对齐”。

```csharp
public ShapeTextVerticalAlignmentType ShapeTextVerticalAlignment { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyShapeTextVerticalAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Aspose.Cells.Drawing.Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 200, 200, 400);
            textBox.Text = "Vertical Alignment Example";
            
            textBox.TextBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Top;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* enum [ShapeTextVerticalAlignmentType](../../shapetextverticalalignmenttype/)
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


