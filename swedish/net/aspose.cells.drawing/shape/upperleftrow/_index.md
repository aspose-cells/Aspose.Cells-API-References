---
title: "Shape.UpperLeftRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar det översta radindexet"
type: docs
url: /sv/net/aspose.cells.drawing/shape/upperleftrow/
---
## Shape.UpperLeftRow property

Representerar det översta radindexet.

```csharp
public int UpperLeftRow { get; set; }
```

### Anmärkningar

Om formen är i formen eller i gruppen, kommer UpperLeftRow att ignoreras.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperLeftRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Ställ in och demonstrera UpperLeftRow-egenskapen
            shape.UpperLeftRow = 3;
            Console.WriteLine("Shape's initial topRow: " + shape.UpperLeftRow);

            // Modifiera UpperLeftRow baserat på villkor
            if (shape.UpperLeftRow == 3)
                shape.UpperLeftRow = 1;

            Console.WriteLine("Shape's modified topRow: " + shape.UpperLeftRow);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


