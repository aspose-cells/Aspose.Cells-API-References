---
title: "Shape.ThreeDFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape property. Hämtar och anger 3D-format för shape"
type: docs
url: /sv/net/aspose.cells.drawing/shape/threedformat/
---
## Shape.ThreeDFormat property

Hämtar och anger 3D-formatet för formen.

```csharp
public ThreeDFormat ThreeDFormat { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyThreeDFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelform med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            // Kom åt och ändra 3D-formatets egenskaper
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.ExtrusionColor.Color = System.Drawing.Color.Blue;
            threeDFormat.LightAngle = 45;
            threeDFormat.ContourWidth = 2;
            threeDFormat.ContourColor.Color = System.Drawing.Color.Red;

            // Spara arbetsboken
            workbook.Save("ThreeDFormatDemo.xlsx");
        }
    }
}
```

### Se även

* class [ThreeDFormat](../../threedformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


