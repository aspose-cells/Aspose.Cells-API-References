---
title: "Shape.WidthCM"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Stellt die Breite der Form in Zentimetern dar"
type: docs
url: /de/net/aspose.cells.drawing/shape/widthcm/
---
## Shape.WidthCM property

Stellt die Breite der Form in Zentimetern dar.

```csharp
public double WidthCM { get; set; }
```

### Beispiele

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

            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 100, 100);

            // Setze die Breite in Zentimetern
            shape.WidthCM = 3.5;
            Console.WriteLine("Shape width set to: " + shape.WidthCM + " cm");

            // Breite ändern, wenn sie einer Bedingung entspricht
            if (shape.WidthCM == 3.5)
            {
                shape.WidthCM = 2.0;
                Console.WriteLine("Shape width changed to: " + shape.WidthCM + " cm");
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


