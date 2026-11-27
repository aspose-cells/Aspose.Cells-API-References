---
title: "Shape.Width"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar formens bredd i enheten pixlar"
type: docs
url: /sv/net/aspose.cells.drawing/shape/width/
---
## Shape.Width property

Representerar formens bredd, i enheten pixlar.

```csharp
public int Width { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform med korrekta parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 50);

            // Ställ in initial bredd och visa den
            shape.Width = 300;
            Console.WriteLine("Initial width: " + shape.Width);

            // Ändra bredden baserat på villkor
            if (shape.Width == 300)
                shape.Width = 150;

            Console.WriteLine("Modified width: " + shape.Width);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


