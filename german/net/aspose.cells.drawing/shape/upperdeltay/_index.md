---
title: "Shape.UpperDeltaY"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den vertikalen Abstand der Form von ihrer oberen linken Ecke zurück oder legt ihn fest."
type: docs
url: /de/net/aspose.cells.drawing/shape/upperdeltay/
---
## Shape.UpperDeltaY property

Liest oder setzt den vertikalen Versatz der Form von ihrer oberen linken Eckzeile.

```csharp
public int UpperDeltaY { get; set; }
```

### Hinweise

Der Wertebereich liegt zwischen 0 und 256.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperDeltaYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Form hinzu, um die UpperDeltaY-Eigenschaft zu demonstrieren.
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Setze und zeige den anfänglichen UpperDeltaY-Wert an.
            shape.UpperDeltaY = 3;
            Console.WriteLine("Initial UpperDeltaY: " + shape.UpperDeltaY);

            // UpperDeltaY-Wert ändern.
            if (shape.UpperDeltaY == 3)
            {
                shape.UpperDeltaY = 1;
                Console.WriteLine("Modified UpperDeltaY: " + shape.UpperDeltaY);
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


