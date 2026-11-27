---
title: "TextBoxOptions.ShapeTextVerticalAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxOptions-egenskap. Den motsvarar Format Shape  Text Options  Text Box  Vertical Alignment i Excel"
type: docs
url: /sv/net/aspose.cells.drawing.texts/textboxoptions/shapetextverticalalignment/
---
## TextBoxOptions.ShapeTextVerticalAlignment property

Det motsvarar "Format Shape - Text Options - Text Box - Vertical Alignment" i Excel.

```csharp
public ShapeTextVerticalAlignmentType ShapeTextVerticalAlignment { get; set; }
```

### Exempel

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

### Se även

* enum [ShapeTextVerticalAlignmentType](../../shapetextverticalalignmenttype/)
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


