---
title: "Shape.WidthInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Stellt die Breite der Form in Zoll dar"
type: docs
url: /de/net/aspose.cells.drawing/shape/widthinch/
---
## Shape.WidthInch property

Stellt die Breite der Form in Zoll dar.

```csharp
public double WidthInch { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform mit allen erforderlichen Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Setze die Breite in Zoll
            shape.WidthInch = 3;
            Console.WriteLine("Shape width (inches): " + shape.WidthInch);

            // Breite ändern, wenn die Bedingung erfüllt ist
            if (shape.WidthInch == 3)
            {
                shape.WidthInch = 1;
                Console.WriteLine("Modified shape width (inches): " + shape.WidthInch);
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


