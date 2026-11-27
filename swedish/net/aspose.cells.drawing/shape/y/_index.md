---
title: "Shape.Y"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Hämtar och anger shape:s vertikala offset från kalkylbladets övre kant i pixelenheter"
type: docs
url: /sv/net/aspose.cells.drawing/shape/y/
---
## Shape.Y property

Hämtar och anger det vertikala offsetet för formen från kalkylbladets övre kant, i enhet pixlar.

```csharp
public int Y { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyYDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Ställ in och demonstrera Y‑egenskapen
            shape.Y = 200;
            Console.WriteLine("Shape Y position: " + shape.Y);

            // Ändra Y‑position baserat på villkor
            if (shape.Y == 200)
                shape.Y = 100;

            Console.WriteLine("Updated Shape Y position: " + shape.Y);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


