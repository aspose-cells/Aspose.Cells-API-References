---
title: "TextBoxOptions.ShapeTextVerticalAlignment"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextBoxOptions. Corrisponde a Formato Forma Opzioni Testo Casella di Testo Allineamento Verticale in Excel"
type: docs
url: /it/net/aspose.cells.drawing.texts/textboxoptions/shapetextverticalalignment/
---
## TextBoxOptions.ShapeTextVerticalAlignment property

Corrisponde a "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel.

```csharp
public ShapeTextVerticalAlignmentType ShapeTextVerticalAlignment { get; set; }
```

### Esempi

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

### Vedi anche

* enum [ShapeTextVerticalAlignmentType](../../shapetextverticalalignmenttype/)
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


