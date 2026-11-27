---
title: "Shape.UpperDeltaY"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar eller anger formens vertikala avstånd från dess övre vänstra rad."
type: docs
url: /sv/net/aspose.cells.drawing/shape/upperdeltay/
---
## Shape.UpperDeltaY property

Hämtar eller anger formens vertikala avstånd från dess övre vänstra hörnrad.

```csharp
public int UpperDeltaY { get; set; }
```

### Anmärkningar

Värdeintervallet är 0 till 256.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperDeltaYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera UpperDeltaY-egenskapen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Ställ in och visa initialt UpperDeltaY-värde
            shape.UpperDeltaY = 3;
            Console.WriteLine("Initial UpperDeltaY: " + shape.UpperDeltaY);

            // Modifiera UpperDeltaY-värdet
            if (shape.UpperDeltaY == 3)
            {
                shape.UpperDeltaY = 1;
                Console.WriteLine("Modified UpperDeltaY: " + shape.UpperDeltaY);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


