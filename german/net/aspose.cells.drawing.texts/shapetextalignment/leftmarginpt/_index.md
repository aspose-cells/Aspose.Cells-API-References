---
title: "ShapeTextAlignment.LeftMarginPt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeTextAlignment-Eigenschaft. Gibt den linken Rand in der Einheit Punkte zurück"
type: docs
url: /de/net/aspose.cells.drawing.texts/shapetextalignment/leftmarginpt/
---
## ShapeTextAlignment.LeftMarginPt property

Gibt den linken Rand in der Einheit Punkte zurück

```csharp
public double LeftMarginPt { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyLeftMarginPtDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform mit allen erforderlichen Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            
            // Setzen Sie den Text für das Shape
            shape.Text = "Sample text with left margin";

            // Zugriff auf die Textausrichtung und Festlegen des linken Randes in Punkten
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            textAlignment.LeftMarginPt = 2.0d;

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeTextAlignmentLeftMarginPtDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


