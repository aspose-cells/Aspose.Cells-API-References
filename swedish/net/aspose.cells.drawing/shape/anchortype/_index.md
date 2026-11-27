---
title: "Shape.AnchorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Hämtar och sätter typen av formens ankare‑platshållare"
type: docs
url: /sv/net/aspose.cells.drawing/shape/anchortype/
---
## Shape.AnchorType property

Hämtar och anger typen av platshållaren för formankaret.

```csharp
public ShapeAnchorType AnchorType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAnchorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form med standardankare‑typ
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
            
            // Kontrollera och ändra ankare‑typ
            if (shape.AnchorType == ShapeAnchorType.OneCellAnchor)
            {
                shape.AnchorType = ShapeAnchorType.TwoCellAnchor;
                Console.WriteLine("Anchor type changed to TwoCellAnchor");
            }
            
            // Spara arbetsboken
            workbook.Save("ShapeAnchorTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ShapeAnchorType](../../shapeanchortype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


