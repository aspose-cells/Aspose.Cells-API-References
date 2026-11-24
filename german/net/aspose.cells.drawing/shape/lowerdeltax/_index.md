---
title: "Shape.LowerDeltaX"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den horizontalen Versatz der Shape von ihrer unteren rechten Eckspalte zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/shape/lowerdeltax/
---
## Shape.LowerDeltaX property

Liest oder setzt den horizontalen Versatz der Form von ihrer unteren rechten Eckspalte.

```csharp
public int LowerDeltaX { get; set; }
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
    public class ShapePropertyLowerDeltaXDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Setzen und Demonstrieren der LowerDeltaX-Eigenschaft
            shape.LowerDeltaX = 3;
            Console.WriteLine("Initial LowerDeltaX: " + shape.LowerDeltaX);

            // LowerDeltaX ändern, wenn die Bedingung erfüllt ist
            if (shape.LowerDeltaX == 3)
            {
                shape.LowerDeltaX = 1;
                Console.WriteLine("Modified LowerDeltaX: " + shape.LowerDeltaX);
            }
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


