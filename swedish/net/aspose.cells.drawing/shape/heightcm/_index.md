---
title: "Shape.HeightCM"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar höjden på formen i enheten centimeter"
type: docs
url: /sv/net/aspose.cells.drawing/shape/heightcm/
---
## Shape.HeightCM property

Representerar formens höjd, i enheten centimeter.

```csharp
public double HeightCM { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangel med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Ställ in höjd i centimeter
            shape.HeightCM = 3;
            Console.WriteLine("Shape height: " + shape.HeightCM + " cm");

            // Ändra höjd om den är 3 cm
            if (shape.HeightCM == 3)
            {
                shape.HeightCM = 1;
                Console.WriteLine("Modified shape height: " + shape.HeightCM + " cm");
            }
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


