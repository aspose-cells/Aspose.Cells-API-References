---
title: "Shape.LowerDeltaX"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar eller anger figurens horisontella förskjutning från dess nedre högra hörnkolumn"
type: docs
url: /sv/net/aspose.cells.drawing/shape/lowerdeltax/
---
## Shape.LowerDeltaX property

Hämtar eller anger formens horisontella förskjutning från dess nedre högra hörnkolumn.

```csharp
public int LowerDeltaX { get; set; }
```

### Anmärkningar

Värdeintervallet är 0 till 1024.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLowerDeltaXDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Ställ in och demonstrera LowerDeltaX-egenskapen
            shape.LowerDeltaX = 3;
            Console.WriteLine("Initial LowerDeltaX: " + shape.LowerDeltaX);

            // Ändra LowerDeltaX om villkoret är uppfyllt
            if (shape.LowerDeltaX == 3)
            {
                shape.LowerDeltaX = 1;
                Console.WriteLine("Modified LowerDeltaX: " + shape.LowerDeltaX);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


