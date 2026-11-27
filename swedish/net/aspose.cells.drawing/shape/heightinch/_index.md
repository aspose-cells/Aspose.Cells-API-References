---
title: "Shape.HeightInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar formens höjd i tum"
type: docs
url: /sv/net/aspose.cells.drawing/shape/heightinch/
---
## Shape.HeightInch property

Representerar figurens höjd, i enhet tum.

```csharp
public double HeightInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangel med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Ange och hämta höjd i tum
            shape.HeightInch = 3;
            Console.WriteLine("Shape height (inches): " + shape.HeightInch);

            // Modifiera höjden om villkoret är uppfyllt
            if (shape.HeightInch == 3)
            {
                shape.HeightInch = 1;
                Console.WriteLine("Modified shape height (inches): " + shape.HeightInch);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


