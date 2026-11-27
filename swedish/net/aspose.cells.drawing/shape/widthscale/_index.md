---
title: "Shape.WidthScale"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar och anger breddskalan i procentenhet av den ursprungliga bildens bredd. Om formen inte är en bild returnerar WidthScale-egenskapen endast 100"
type: docs
url: /sv/net/aspose.cells.drawing/shape/widthscale/
---
## Shape.WidthScale property

Hämtar och anger breddskalan, i enhet procent av den ursprungliga bildens bredd. Om formen inte är en bild, returnerar WidthScale‑egenskapen endast 100;

```csharp
public int WidthScale { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthScaleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform med korrekta parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Ställ in initial breddskala
            shape.WidthScale = 50;
            Console.WriteLine("Initial WidthScale: " + shape.WidthScale);

            // Ändra breddskala om villkoret uppfylls
            if (shape.WidthScale == 50)
            {
                shape.WidthScale = 75;
                Console.WriteLine("Updated WidthScale: " + shape.WidthScale);
            }

            // Spara arbetsboken
            workbook.Save("ShapeWidthScaleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


