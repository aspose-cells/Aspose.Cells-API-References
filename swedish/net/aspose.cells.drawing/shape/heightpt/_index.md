---
title: "Shape.HeightPt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar formens höjd i enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing/shape/heightpt/
---
## Shape.HeightPt property

Representerar figurens höjd, i enhet punkter.

```csharp
public double HeightPt { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelform med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 100);

            // Ange och hämta HeightPt-egenskapen
            shape.HeightPt = 50;
            Console.WriteLine("Shape height in points: " + shape.HeightPt);

            // Ändra höjden om den uppfyller ett villkor
            if (shape.HeightPt == 50)
            {
                shape.HeightPt = 30;
                Console.WriteLine("Modified shape height: " + shape.HeightPt);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


