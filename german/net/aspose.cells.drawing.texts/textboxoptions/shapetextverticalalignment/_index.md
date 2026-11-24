---
title: "TextBoxOptions.ShapeTextVerticalAlignment"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxOptions-Eigenschaft. Sie entspricht Format Shape  Text Options  Text Box  Vertical Alignment in Excel"
type: docs
url: /de/net/aspose.cells.drawing.texts/textboxoptions/shapetextverticalalignment/
---
## TextBoxOptions.ShapeTextVerticalAlignment property

Entspricht "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel.

```csharp
public ShapeTextVerticalAlignmentType ShapeTextVerticalAlignment { get; set; }
```

### Beispiele

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

### Siehe auch

* enum [ShapeTextVerticalAlignmentType](../../shapetextverticalalignmenttype/)
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


