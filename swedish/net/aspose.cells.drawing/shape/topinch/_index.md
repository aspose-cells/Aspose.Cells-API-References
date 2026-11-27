---
title: "Shape.TopInch"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar den vertikala förskjutningen av formen från dess översta rad i tum"
type: docs
url: /sv/net/aspose.cells.drawing/shape/topinch/
---
## Shape.TopInch property

Representerar figurens vertikala förskjutning från dess översta rad, i tum.

```csharp
public double TopInch { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopInchDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Ställ in och demonstrera egenskapen TopInch
            shape.TopInch = 3;
            Console.WriteLine("Shape Top position (inches): " + shape.TopInch);

            // Modifiera TopInch om den är lika med 3
            if (shape.TopInch == 3)
            {
                shape.TopInch = 1;
                Console.WriteLine("Modified Shape Top position (inches): " + shape.TopInch);
            }

            // Spara arbetsboken
            workbook.Save("ShapeTopInchDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


