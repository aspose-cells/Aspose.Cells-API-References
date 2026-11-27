---
title: "Shape.ActualLowerRightRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape egenskap. Hämta den faktiska nedersta raden"
type: docs
url: /sv/net/aspose.cells.drawing/shape/actuallowerrightrow/
---
## Shape.ActualLowerRightRow property

Hämta den faktiska sista raden.

```csharp
public int ActualLowerRightRow { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyActualLowerRightRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelform (rektangel)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 100);

            // Hämta den faktiska nedre högra raden för formen
            int actualLowerRightRow = shape.ActualLowerRightRow;

            // Skriv ut resultatet
            Console.WriteLine("Actual Lower Right Row of the shape: " + actualLowerRightRow);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


