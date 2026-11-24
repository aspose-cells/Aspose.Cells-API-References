---
title: "Shape.UpperDeltaX"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den horizontalen Versatz der Form von ihrer oberen linken Spalte zurück oder legt ihn fest."
type: docs
url: /de/net/aspose.cells.drawing/shape/upperdeltax/
---
## Shape.UpperDeltaX property

Liest oder setzt den horizontalen Versatz der Form von ihrer oberen linken Eckspalte.

```csharp
public int UpperDeltaX { get; set; }
```

### Hinweise

Der Wertebereich liegt zwischen 0 und 1024.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperDeltaXDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Setze und zeige die UpperDeltaX-Eigenschaft.
            shape.UpperDeltaX = 150;
            Console.WriteLine("UpperDeltaX: " + shape.UpperDeltaX);

            // Ändere die UpperDeltaX, wenn sie eine Bedingung erfüllt.
            if (shape.UpperDeltaX == 150)
            {
                shape.UpperDeltaX = 100;
                Console.WriteLine("Modified UpperDeltaX: " + shape.UpperDeltaX);
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


