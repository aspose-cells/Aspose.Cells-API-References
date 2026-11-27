---
title: "Shape.TopToCorner"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar och anger det vertikala avståndet för formen från kalkylbladets övre kant i pixlar"
type: docs
url: /sv/net/aspose.cells.drawing/shape/toptocorner/
---
## Shape.TopToCorner property

Hämtar och anger figurens vertikala förskjutning från kalkylbladets övre kant, i pixlar.

```csharp
public int TopToCorner { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopToCornerDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform i arbetsbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Ange och visa TopToCorner-egenskapen
            shape.TopToCorner = 50;
            Console.WriteLine("Shape TopToCorner: " + shape.TopToCorner);

            // Modifiera TopToCorner-egenskapen
            if (shape.TopToCorner == 50)
            {
                shape.TopToCorner = 20;
                Console.WriteLine("Updated Shape TopToCorner: " + shape.TopToCorner);
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


