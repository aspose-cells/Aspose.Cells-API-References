---
title: "Shape.Title"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑egenskap. Anger titelrubriken för det aktuella shape‑objektet"
type: docs
url: /sv/net/aspose.cells.drawing/shape/title/
---
## Shape.Title property

Anger titeln (rubriken) för det aktuella formobjektet.

```csharp
public string Title { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTitleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangel med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Ställ in titeln för shape
            shape.Title = "title1";

            // Verifiera att titeln har satts
            Console.WriteLine("Shape title: " + shape.Title);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


