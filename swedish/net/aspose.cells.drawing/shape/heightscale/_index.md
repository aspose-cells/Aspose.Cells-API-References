---
title: "Shape.HeightScale"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar och anger höjds skalan i enheten procent av den ursprungliga bildens höjd. Om formen inte är en bild returnerar HeightScale property endast 100"
type: docs
url: /sv/net/aspose.cells.drawing/shape/heightscale/
---
## Shape.HeightScale property

Hämtar och anger höjds‑skalan, i procent av den ursprungliga bildens höjd. Om figuren inte är en bild, returnerar HeightScale‑egenskapen endast 100;

```csharp
public int HeightScale { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightScaleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 150);

            // Ställ in initial höjds skala
            shape.HeightScale = 50;
            Console.WriteLine("Initial HeightScale: " + shape.HeightScale);

            // Ändra höjds skala om villkoret är uppfyllt
            if (shape.HeightScale == 50)
            {
                shape.HeightScale = 75;
                Console.WriteLine("Modified HeightScale: " + shape.HeightScale);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


