---
title: "ShapeTextAlignment.RotationAngle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeTextAlignment Eigenschaft. Liest und setzt die Drehung der Form"
type: docs
url: /de/net/aspose.cells.drawing.texts/shapetextalignment/rotationangle/
---
## ShapeTextAlignment.RotationAngle property

Liest und setzt die Drehung der Form.

```csharp
public double RotationAngle { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRotationAngleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 200, 300, 400);
            
            // Formtext festlegen
            shape.Text = "Rotated Text";
            
            // Zugriff auf die Textausrichtung und Setzen des Rotationswinkels
            shape.TextBody.TextAlignment.RotationAngle = 90;

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeTextRotationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


