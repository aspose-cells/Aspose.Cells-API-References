---
title: "Shape.Bottom"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Representerar bredden på figurens vertikala förskjutning från dess nedre hörnrad i enheten pixlar"
type: docs
url: /sv/net/aspose.cells.drawing/shape/bottom/
---
## Shape.Bottom property

Representerar bredden på formens vertikala förskjutning från dess nedre hörnrad, i enheten pixlar.

```csharp
public int Bottom { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyBottomDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelform med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Ställ in initial position
            shape.Top = 200;
            shape.Left = 200;

            // Demonstrera Bottom‑egenskapen
            Console.WriteLine("Original Bottom position: " + shape.Bottom);

            // Ändra Bottom‑positionen
            if (shape.Bottom == 300)  // 200 (Top) + 100 (Height)
            {
                shape.Bottom = 250;  // This will change the Top position (250 - 100 = 150)
                Console.WriteLine("New Bottom position: " + shape.Bottom);
                Console.WriteLine("New Top position: " + shape.Top);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


