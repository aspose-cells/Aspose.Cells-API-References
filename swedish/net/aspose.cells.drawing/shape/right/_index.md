---
title: "Shape.Right"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Representerar bredden på formens horisontella förskjutning från dess nedre högra hörnkolumn i pixelenheter"
type: docs
url: /sv/net/aspose.cells.drawing/shape/right/
---
## Shape.Right property

Representerar bredden på formens horisontella förskjutning från dess nedre högra hörnkolumn, i enheten pixlar.

```csharp
public int Right { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRightDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Ange och hämta Right‑egenskapen
            shape.Right = 200;
            Console.WriteLine("Shape Right position: " + shape.Right);

            // Ändra Right‑egenskapen villkorligt
            if (shape.Right == 200)
                shape.Right = 150;

            Console.WriteLine("Modified Shape Right position: " + shape.Right);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


