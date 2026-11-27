---
title: "Shape.LeftToCorner"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Hämtar och anger den horisontella förskjutningen av formen från kalkylbladets vänstra kant"
type: docs
url: /sv/net/aspose.cells.drawing/shape/lefttocorner/
---
## Shape.LeftToCorner property

Hämtar och anger den horisontella förskjutningen av figuren från kalkylbladets vänstra kant.

```csharp
public int LeftToCorner { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftToCornerDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform med korrekta parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Ange och demonstrera LeftToCorner‑egenskapen
            shape.LeftToCorner = 50;
            Console.WriteLine("Shape LeftToCorner value: " + shape.LeftToCorner);

            // Ändra LeftToCorner om den är lika med ett specifikt värde
            if (shape.LeftToCorner == 50)
            {
                shape.LeftToCorner = 30;
                Console.WriteLine("Modified LeftToCorner value: " + shape.LeftToCorner);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


