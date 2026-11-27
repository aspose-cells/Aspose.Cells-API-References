---
title: "Shape.WidthInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar formens bredd i tum"
type: docs
url: /sv/net/aspose.cells.drawing/shape/widthinch/
---
## Shape.WidthInch property

Representerar bredden på formen, i enhet tum.

```csharp
public double WidthInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangel med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Ange bredd i tum
            shape.WidthInch = 3;
            Console.WriteLine("Shape width (inches): " + shape.WidthInch);

            // Ändra bredd om villkoret är uppfyllt
            if (shape.WidthInch == 3)
            {
                shape.WidthInch = 1;
                Console.WriteLine("Modified shape width (inches): " + shape.WidthInch);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


