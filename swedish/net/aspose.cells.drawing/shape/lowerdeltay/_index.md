---
title: "Shape.LowerDeltaY"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar eller anger formens vertikala förskjutning från dess nedre högra hörnrad"
type: docs
url: /sv/net/aspose.cells.drawing/shape/lowerdeltay/
---
## Shape.LowerDeltaY property

Hämtar eller anger formens vertikala förskjutning från dess nedre högra hörnrad.

```csharp
public int LowerDeltaY { get; set; }
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
    public class ShapePropertyLowerDeltaYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelform med korrekta parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Ange och demonstrera LowerDeltaY-egenskapen
            shape.LowerDeltaY = 20;
            Console.WriteLine("Initial LowerDeltaY: " + shape.LowerDeltaY);

            // Modifiera LowerDeltaY villkorligt
            if (shape.LowerDeltaY == 20)
            {
                shape.LowerDeltaY = 10;
                Console.WriteLine("Modified LowerDeltaY: " + shape.LowerDeltaY);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


