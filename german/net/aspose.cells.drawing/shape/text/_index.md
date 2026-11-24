---
title: "Shape.Text"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den Text dieser Form zurück und setzt ihn"
type: docs
url: /de/net/aspose.cells.drawing/shape/text/
---
## Shape.Text property

Liest und setzt den Text dieser Form.

```csharp
public string Text { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Rechteck shape mit korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Setze Text, falls null
            if (shape.Text == null)
            {
                shape.Text = "This is a test.";
            }

            // Ändere den Text
            shape.Text = "Updated text demo";

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeTextDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


