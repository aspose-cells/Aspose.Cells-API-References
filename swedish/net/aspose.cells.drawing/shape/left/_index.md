---
title: "Shape.Left"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar den horisontella förskjutningen av formen från dess vänstra kolumn i pixlar"
type: docs
url: /sv/net/aspose.cells.drawing/shape/left/
---
## Shape.Left property

Representerar den horisontella förskjutningen av figuren från dess vänstra kolumn, i enhet pixlar.

```csharp
public int Left { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera Left-egenskapen
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Ange initial Left-position
            shape.Left = 200;
            Console.WriteLine("Shape Left position: " + shape.Left);

            // Ändra Left-positionen villkorligt
            if (shape.Left == 200)
            {
                shape.Left = 150;
                Console.WriteLine("Adjusted Shape Left position: " + shape.Left);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


