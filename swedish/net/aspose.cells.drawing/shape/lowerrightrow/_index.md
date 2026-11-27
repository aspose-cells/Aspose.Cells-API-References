---
title: "Shape.LowerRightRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar radindex för nedre högra hörnet"
type: docs
url: /sv/net/aspose.cells.drawing/shape/lowerrightrow/
---
## Shape.LowerRightRow property

Representerar radindex för nedre högra hörnet.

```csharp
public int LowerRightRow { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLowerRightRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Ställ in och demonstrera egenskapen LowerRightRow
            Console.WriteLine("Original LowerRightRow: " + shape.LowerRightRow);
            shape.LowerRightRow = 3;
            Console.WriteLine("Modified LowerRightRow: " + shape.LowerRightRow);

            // Villkorlig modifiering enligt testfall
            if (shape.LowerRightRow == 3)
            {
                shape.LowerRightRow = 1;
                Console.WriteLine("Final LowerRightRow after condition: " + shape.LowerRightRow);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


