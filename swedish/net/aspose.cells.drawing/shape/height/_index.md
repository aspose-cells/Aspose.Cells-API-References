---
title: "Shape.Height"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape property. Representerar formens höjd i enheten pixel"
type: docs
url: /sv/net/aspose.cells.drawing/shape/height/
---
## Shape.Height property

Representerar formens höjd, i enheten pixlar.

```csharp
public int Height { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangel med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Ange initial höjd
            shape.Height = 150;
            Console.WriteLine("Initial height: " + shape.Height);

            // Modifiera höjden villkorsmässigt
            if (shape.Height == 150)
            {
                shape.Height = 100;
                Console.WriteLine("Modified height: " + shape.Height);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


