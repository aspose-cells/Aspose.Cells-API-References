---
title: "Shape.UpperDeltaX"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar eller anger formens horisontella avstånd från dess övre vänstra kolumn"
type: docs
url: /sv/net/aspose.cells.drawing/shape/upperdeltax/
---
## Shape.UpperDeltaX property

Hämtar eller anger formens horisontella avstånd från dess övre vänstra hörnkolumn.

```csharp
public int UpperDeltaX { get; set; }
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
    public class ShapePropertyUpperDeltaXDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Ange och visa UpperDeltaX-egenskapen
            shape.UpperDeltaX = 150;
            Console.WriteLine("UpperDeltaX: " + shape.UpperDeltaX);

            // Modifiera UpperDeltaX om det uppfyller ett villkor
            if (shape.UpperDeltaX == 150)
            {
                shape.UpperDeltaX = 100;
                Console.WriteLine("Modified UpperDeltaX: " + shape.UpperDeltaX);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


