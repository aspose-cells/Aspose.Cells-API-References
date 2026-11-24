---
title: "Shape.ThreeDFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape Eigenschaft. Liest und schreibt das 3D-Format der Form."
type: docs
url: /de/net/aspose.cells.drawing/shape/threedformat/
---
## Shape.ThreeDFormat property

Liest und setzt das 3D-Format der Form.

```csharp
public ThreeDFormat ThreeDFormat { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyThreeDFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispielhafte Form mit allen erforderlichen Parametern hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            // Auf 3D-Formateigenschaften zugreifen und sie ändern
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.ExtrusionColor.Color = System.Drawing.Color.Blue;
            threeDFormat.LightAngle = 45;
            threeDFormat.ContourWidth = 2;
            threeDFormat.ContourColor.Color = System.Drawing.Color.Red;

            // Speichere die Arbeitsmappe
            workbook.Save("ThreeDFormatDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThreeDFormat](../../threedformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


