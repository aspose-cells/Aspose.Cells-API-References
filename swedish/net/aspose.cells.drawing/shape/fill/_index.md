---
title: "Shape.Fill"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape property. Returnerar ett FillFormat-objekt som innehåller fyllningsformateringsegenskaper för den angivna shape"
type: docs
url: /sv/net/aspose.cells.drawing/shape/fill/
---
## Shape.Fill property

Returnerar ett [`FillFormat`](../fillformat/) objekt som innehåller fyllningsformateringsegenskaper för den angivna shape.

```csharp
public FillFormat Fill { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFillDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform med korrekta parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Hämta fyllningsformatet för formen
            FillFormat fillFmt = shape.Fill;

            // Ange solid fyllning med färg
            fillFmt.SolidFill.Color = System.Drawing.Color.Red;

            // Ställ in transparens
            fillFmt.Transparency = 0.5;

            // Spara arbetsboken
            workbook.Save("ShapeFillDemo.xlsx");
        }
    }
}
```

### Se även

* class [FillFormat](../../fillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


