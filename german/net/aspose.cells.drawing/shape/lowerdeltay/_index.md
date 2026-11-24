---
title: "Shape.LowerDeltaY"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den vertikalen Versatz des Shapes von seiner unteren rechten Ecke zurück oder setzt ihn"
type: docs
url: /de/net/aspose.cells.drawing/shape/lowerdeltay/
---
## Shape.LowerDeltaY property

Liest oder setzt den vertikalen Versatz der Form von ihrer unteren rechten Eckzeile.

```csharp
public int LowerDeltaY { get; set; }
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
    public class ShapePropertyLowerDeltaYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein Beispiel-Shape mit den korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Setzen und demonstrieren Sie die LowerDeltaY-Eigenschaft
            shape.LowerDeltaY = 20;
            Console.WriteLine("Initial LowerDeltaY: " + shape.LowerDeltaY);

            // Ändern Sie LowerDeltaY bedingt
            if (shape.LowerDeltaY == 20)
            {
                shape.LowerDeltaY = 10;
                Console.WriteLine("Modified LowerDeltaY: " + shape.LowerDeltaY);
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


