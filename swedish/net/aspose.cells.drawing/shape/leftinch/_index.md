---
title: "Shape.LeftInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar den horisontella förskjutningen av formen från dess vänstra kolumn i enheten tum"
type: docs
url: /sv/net/aspose.cells.drawing/shape/leftinch/
---
## Shape.LeftInch property

Representerar den horisontella förskjutningen av figuren från dess vänstra kolumn, i enhet tum.

```csharp
public double LeftInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelform med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Ställ in och demonstrera LeftInch-egenskapen
            shape.LeftInch = 3;
            Console.WriteLine("Shape left position (inches): " + shape.LeftInch);

            // Ändra vänsterposition om den är 3 tum
            if (shape.LeftInch == 3)
            {
                shape.LeftInch = 1;
                Console.WriteLine("Adjusted shape left position (inches): " + shape.LeftInch);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


