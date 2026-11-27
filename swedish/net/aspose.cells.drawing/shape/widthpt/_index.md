---
title: "Shape.WidthPt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar bredden på formen i enheten punkt"
type: docs
url: /sv/net/aspose.cells.drawing/shape/widthpt/
---
## Shape.WidthPt property

Representerar bredden på formen, i enhet punkt.

```csharp
public double WidthPt { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthPtDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Ange och hämta bredden i punkter
            shape.WidthPt = 150;
            Console.WriteLine("Shape width in points: " + shape.WidthPt);

            // Ändra bredd om villkoret är uppfyllt
            if (shape.WidthPt == 150)
            {
                shape.WidthPt = 100;
                Console.WriteLine("Modified shape width in points: " + shape.WidthPt);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


