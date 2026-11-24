---
title: "Shape.Y"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den vertikalen Versatz des Shapes vom oberen Rand des Arbeitsblatts in Pixeln zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/shape/y/
---
## Shape.Y property

Liest und setzt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts, in Einheit Pixel.

```csharp
public int Y { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyYDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Setzen und demonstrieren Sie die Y-Eigenschaft
            shape.Y = 200;
            Console.WriteLine("Shape Y position: " + shape.Y);

            // Y-Position basierend auf einer Bedingung ändern
            if (shape.Y == 200)
                shape.Y = 100;

            Console.WriteLine("Updated Shape Y position: " + shape.Y);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


