---
title: "Aufzählung ShapeAnchorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ShapeAnchorType Aufzählung. Stellt den Ankertyp dar"
type: docs
url: /de/net/aspose.cells.drawing/shapeanchortype/
---
## ShapeAnchorType enumeration

Stellt den Ankertyp dar.

```csharp
public enum ShapeAnchorType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| TwoCellAnchor | `0` | Stellt einen Platzhalter für einen Anker mit zwei Zellen dar |
| OneCellAnchor | `1` | Stellt einen Platzhalter für einen Anker mit einer Zelle dar |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapeAnchorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Gruppenfeldform hinzu
            Shape box = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 300, 250);
            box.Text = "Sample Group Box";
            
            // Demonstriere die Verwendung von ShapeAnchorType
            box.AnchorType = ShapeAnchorType.TwoCellAnchor;
            box.UpperLeftRow = 2;
            box.UpperLeftColumn = 1;
            box.LowerRightRow = 8;
            box.LowerRightColumn = 4;

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeAnchorTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


