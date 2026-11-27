---
title: "Shape.TopCM"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Representerar det vertikala avståndet för formen från dess översta rad i enhet av centimeter"
type: docs
url: /sv/net/aspose.cells.drawing/shape/topcm/
---
## Shape.TopCM property

Representerar figurens vertikala förskjutning från dess översta rad, i centimeter.

```csharp
public double TopCM { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            shape.TopCM = 3.0;
            
            Console.WriteLine("Shape Top position (cm): " + shape.TopCM);
            
            if (shape.TopCM == 3.0)
                shape.TopCM = 1.0;
                
            Console.WriteLine("Shape Top position after change (cm): " + shape.TopCM);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


