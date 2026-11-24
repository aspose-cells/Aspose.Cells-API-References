---
title: "ShapeTextAlignment.RightMarginPt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeTextAlignment Eigenschaft. Gibt den rechten Rand in Punkten zurück"
type: docs
url: /de/net/aspose.cells.drawing.texts/shapetextalignment/rightmarginpt/
---
## ShapeTextAlignment.RightMarginPt property

Gibt den rechten Rand in der Einheit Punkte zurück

```csharp
public double RightMarginPt { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRightMarginPtDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform mit allen erforderlichen Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Zugriff auf die Textausrichtung
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Setze den rechten Rand in Punkten
            shapeTextAlignment.RightMarginPt = 2.0d;

            // Überprüfe die Eigenschaft, indem du den Wert zurückholst
            Console.WriteLine("Right Margin in Points: " + shapeTextAlignment.RightMarginPt);
        }
    }
}
```

### Siehe auch

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


