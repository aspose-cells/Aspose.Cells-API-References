---
title: "Shape.UpperLeftColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape property. Representerar kolumnindex för övre vänstra hörnet"
type: docs
url: /sv/net/aspose.cells.drawing/shape/upperleftcolumn/
---
## Shape.UpperLeftColumn property

Representerar kolumnindex för övre vänstra hörnet.

```csharp
public int UpperLeftColumn { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperLeftColumnDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 100);

            // Ange och demonstrera UpperLeftColumn-egenskapen
            shape.UpperLeftColumn = 3;
            Console.WriteLine("Shape's initial leftColumn: " + shape.UpperLeftColumn);

            // Modifiera UpperLeftColumn
            if (shape.UpperLeftColumn == 3)
            {
                shape.UpperLeftColumn = 1;
                Console.WriteLine("Shape's modified leftColumn: " + shape.UpperLeftColumn);
            }

            // Spara arbetsboken
            workbook.Save("ShapeUpperLeftColumnDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


