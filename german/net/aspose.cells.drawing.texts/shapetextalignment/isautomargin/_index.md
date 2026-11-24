---
title: "ShapeTextAlignment.IsAutoMargin"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeTextAlignment-Eigenschaft. Gibt an, ob der Rand des Textrahmens automatisch ist"
type: docs
url: /de/net/aspose.cells.drawing.texts/shapetextalignment/isautomargin/
---
## ShapeTextAlignment.IsAutoMargin property

Gibt an, ob der Rand des Textrahmens automatisch ist.

```csharp
public bool IsAutoMargin { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsAutoMarginDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform mit allen erforderlichen Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Zugriff auf die Textausrichtung und Setzen von IsAutoMargin
            shape.TextBody.TextAlignment.IsAutoMargin = true;

            // Setzen Sie einen Beispieltext
            shape.Text = "Sample text with auto margins";

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeTextAlignmentIsAutoMarginDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


