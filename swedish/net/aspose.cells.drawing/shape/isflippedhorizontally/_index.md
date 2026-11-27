---
title: "Shape.IsFlippedHorizontally"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape property. Hämtar och anger om formen är horisontellt speglad"
type: docs
url: /sv/net/aspose.cells.drawing/shape/isflippedhorizontally/
---
## Shape.IsFlippedHorizontally property

Hämtar och anger om formen är horisontellt speglad.

```csharp
public bool IsFlippedHorizontally { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsFlippedHorizontallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelform med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Kontrollera och vänd horisontellt om den inte redan är vänd
            if (shape.IsFlippedHorizontally == false)
            {
                shape.IsFlippedHorizontally = true;
                Console.WriteLine("Shape was flipped horizontally");
            }
            else
            {
                Console.WriteLine("Shape was already flipped horizontally");
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


