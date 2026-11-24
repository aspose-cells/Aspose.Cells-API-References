---
title: "Shape.TopToCorner"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts in Pixeln zurück und legt ihn fest."
type: docs
url: /de/net/aspose.cells.drawing/shape/toptocorner/
---
## Shape.TopToCorner property

Liest und setzt den vertikalen Versatz der Form vom oberen Rand des Arbeitsblatts, in Einheit Pixel.

```csharp
public int TopToCorner { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Rechteck-Shape zum Arbeitsblatt hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Setze und zeige die TopToCorner-Eigenschaft.
            shape.TopToCorner = 50;
            Console.WriteLine("Shape TopToCorner: " + shape.TopToCorner);

            // Ändere die TopToCorner-Eigenschaft.
            if (shape.TopToCorner == 50)
            {
                shape.TopToCorner = 20;
                Console.WriteLine("Updated Shape TopToCorner: " + shape.TopToCorner);
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


