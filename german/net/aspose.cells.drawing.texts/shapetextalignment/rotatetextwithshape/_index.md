---
title: "ShapeTextAlignment.RotateTextWithShape"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeTextAlignment-Eigenschaft. Gibt an, ob Text mit der Form rotiert wird"
type: docs
url: /de/net/aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape/
---
## ShapeTextAlignment.RotateTextWithShape property

Gibt an, ob Text mit einer Form rotiert wird

```csharp
public bool RotateTextWithShape { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRotateTextWithShapeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Textfeld-Form mit korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            shape.Text = "Sample Text";

            // Zugriff auf Textausrichtungs-Eigenschaften
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            
            // Setzen Sie die RotateTextWithShape-Eigenschaft
            textAlignment.RotateTextWithShape = true;

            // Rotieren Sie die Form, um den Effekt zu demonstrieren
            shape.RotationAngle = 45;

            // Speichere die Arbeitsmappe
            workbook.Save("RotateTextWithShapeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


