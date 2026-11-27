---
title: "Shape.WidthCM"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar formens bredd i centimeter"
type: docs
url: /sv/net/aspose.cells.drawing/shape/widthcm/
---
## Shape.WidthCM property

Representerar bredden på formen, i enhet centimeter.

```csharp
public double WidthCM { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 100, 100);

            // Ange bredd i centimeter
            shape.WidthCM = 3.5;
            Console.WriteLine("Shape width set to: " + shape.WidthCM + " cm");

            // Ändra bredden om den matchar ett villkor
            if (shape.WidthCM == 3.5)
            {
                shape.WidthCM = 2.0;
                Console.WriteLine("Shape width changed to: " + shape.WidthCM + " cm");
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


