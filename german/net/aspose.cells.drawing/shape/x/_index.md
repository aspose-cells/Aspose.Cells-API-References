---
title: "Shape.X"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Liest und setzt den horizontalen Versatz des shape vom linken Rand des Arbeitsblatts in Pixeln"
type: docs
url: /de/net/aspose.cells.drawing/shape/x/
---
## Shape.X property

Liest und setzt den horizontalen Versatz der Form vom linken Rand des Arbeitsblatts, in Pixeln.

```csharp
public int X { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyXDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Setze die anfängliche X-Position
            shape.X = 200;
            Console.WriteLine("Initial X position: " + shape.X);

            // Ändere die X-Position, wenn sie 3 beträgt (zur Demonstration der Testfalllogik)
            if (shape.X == 3)
            {
                shape.X = 1;
            }
            else
            {
                // Zur Demonstration ändere die X-Position auf 300
                shape.X = 300;
            }

            Console.WriteLine("Final X position: " + shape.X);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


