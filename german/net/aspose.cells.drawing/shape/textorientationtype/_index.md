---
title: "Shape.TextOrientationType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den Textorientierungstyp des Shapes zurück und setzt ihn"
type: docs
url: /de/net/aspose.cells.drawing/shape/textorientationtype/
---
## Shape.TextOrientationType property

Liest und setzt den Orientierungstyp des Textes in der Form.

```csharp
public TextOrientationType TextOrientationType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextOrientationTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // Setzen Sie den Text für das Shape
            shape.Text = "Sample Text";

            // Überprüfen und ändern Sie die Textorientierung
            if (shape.TextOrientationType == TextOrientationType.NoRotation)
            {
                shape.TextOrientationType = TextOrientationType.TopToBottom;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeTextOrientationDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextOrientationType](../../../aspose.cells/textorientationtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


