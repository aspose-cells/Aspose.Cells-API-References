---
title: "Shape.RotationAngle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar och anger rotationen för formen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/rotationangle/
---
## Shape.RotationAngle property

Hämtar och anger rotationen för formen.

```csharp
public double RotationAngle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangel med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 100, 200, 0, 0);

            // Ställ in rotationsvinkeln till 60 grader
            shape.RotationAngle = 60;
            Console.WriteLine("Shape rotation angle set to: " + shape.RotationAngle);

            // Hämta aktuell rotationsvinkel
            double currentAngle = shape.RotationAngle;
            Console.WriteLine("Current shape rotation angle: " + currentAngle);

            // Spara arbetsboken
            workbook.Save("ShapeRotationDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


