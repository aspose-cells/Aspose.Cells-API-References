---
title: "Shape.AnchorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den Typ des Form-Anker-Platzhalters zurück und legt ihn fest."
type: docs
url: /de/net/aspose.cells.drawing/shape/anchortype/
---
## Shape.AnchorType property

Liest und legt den Typ des Platzhalters für das Shape-Anker fest.

```csharp
public ShapeAnchorType AnchorType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAnchorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Form mit dem Standard-Ankertyp hinzu.
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
            
            // Überprüfen und ändern Sie den Ankertyp.
            if (shape.AnchorType == ShapeAnchorType.OneCellAnchor)
            {
                shape.AnchorType = ShapeAnchorType.TwoCellAnchor;
                Console.WriteLine("Anchor type changed to TwoCellAnchor");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("ShapeAnchorTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ShapeAnchorType](../../shapeanchortype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


