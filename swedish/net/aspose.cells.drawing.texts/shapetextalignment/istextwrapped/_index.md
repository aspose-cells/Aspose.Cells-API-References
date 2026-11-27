---
title: "ShapeTextAlignment.IsTextWrapped"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeTextAlignment-egenskapen. Hämtar eller anger textomslagstypen för formen som innehåller text"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextalignment/istextwrapped/
---
## ShapeTextAlignment.IsTextWrapped property

Hämtar eller anger den textomslutna typen för formen som innehåller text.

```csharp
public bool IsTextWrapped { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangel med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Ange formtext
            shape.Text = "This is a long text that should be wrapped when IsTextWrapped is set to true";

            // Hämta textjustering och ställ in IsTextWrapped
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            shapeTextAlignment.IsTextWrapped = true;

            // Spara arbetsboken
            workbook.Save("ShapeTextWrappingDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


