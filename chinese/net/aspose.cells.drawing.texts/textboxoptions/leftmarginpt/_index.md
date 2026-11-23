---
title: "TextBoxOptions.LeftMarginPt"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TextBoxOptions 属性。获取并设置以点为单位的左边距"
type: docs
url: /zh/net/aspose.cells.drawing.texts/textboxoptions/leftmarginpt/
---
## TextBoxOptions.LeftMarginPt property

获取和设置以点为单位的左侧边距。

```csharp
public double LeftMarginPt { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyLeftMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 400);
            textBox.TextBoxOptions.LeftMarginPt = 0.2d;

            Console.WriteLine("Left margin set to: " + textBox.TextBoxOptions.LeftMarginPt + " points");
        }
    }
}
```

### 另请参见

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


