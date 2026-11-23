---
title: "TextBoxOptions.BottomMarginPt"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TextBoxOptions 属性。返回以点为单位的下边距"
type: docs
url: /zh/net/aspose.cells.drawing.texts/textboxoptions/bottommarginpt/
---
## TextBoxOptions.BottomMarginPt property

返回以点为单位的底部边距

```csharp
public double BottomMarginPt { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyBottomMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            shape.TextBoxOptions.BottomMarginPt = 0.2d;

            Console.WriteLine("Bottom margin set to: " + shape.TextBoxOptions.BottomMarginPt + " points");
        }
    }
}
```

### 另请参见

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


