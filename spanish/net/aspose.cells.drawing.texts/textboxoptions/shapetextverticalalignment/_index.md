---
title: "TextBoxOptions.ShapeTextVerticalAlignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxOptions. Corresponde a Formato de Forma  Opciones de Texto  Cuadro de Texto  Alineación Vertical en Excel"
type: docs
url: /es/net/aspose.cells.drawing.texts/textboxoptions/shapetextverticalalignment/
---
## TextBoxOptions.ShapeTextVerticalAlignment property

Corresponde a "Formato de forma - Opciones de texto - Cuadro de texto - Alineación vertical" en Excel.

```csharp
public ShapeTextVerticalAlignmentType ShapeTextVerticalAlignment { get; set; }
```

### Ejemplos

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

### Ver también

* enum [ShapeTextVerticalAlignmentType](../../shapetextverticalalignmenttype/)
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


