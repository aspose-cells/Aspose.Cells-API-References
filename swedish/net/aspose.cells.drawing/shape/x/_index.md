---
title: "Shape.X"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape egenskap. Hämtar och anger den horisontella förskjutningen av formen från kalkylbladets vänstra kant i pixelenheter"
type: docs
url: /sv/net/aspose.cells.drawing/shape/x/
---
## Shape.X property

Hämtar och anger formens horisontella avstånd från kalkylbladets vänstra kant, i enhet pixlar.

```csharp
public int X { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyXDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Ställ in initial X-position
            shape.X = 200;
            Console.WriteLine("Initial X position: " + shape.X);

            // Ändra X-position om den är lika med 3 (demonstrerar testfallslogiken)
            if (shape.X == 3)
            {
                shape.X = 1;
            }
            else
            {
                // För demonstration, ändra X-position till 300
                shape.X = 300;
            }

            Console.WriteLine("Final X position: " + shape.X);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


