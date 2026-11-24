---
title: "Shape.Line"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den Linienstil zurück"
type: docs
url: /de/net/aspose.cells.drawing/shape/line/
---
## Shape.Line property

Liest den Linienstil

```csharp
public LineFormat Line { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLineDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Linienform hinzufügen (gibt LineShape direkt zurück)
            LineShape lineShape = worksheet.Shapes.AddLine(1, 0, 1, 0, 5, 100);

            // Zugriff auf und Ändern von Linieneigenschaften
            LineFormat lineFormat = lineShape.Line;
            lineFormat.CompoundType = MsoLineStyle.ThickThin;
            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            lineFormat.Weight = 3.0;
            lineFormat.BeginArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineFormat.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Speichere die Arbeitsmappe
            workbook.Save("LineShapeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [LineFormat](../../lineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


