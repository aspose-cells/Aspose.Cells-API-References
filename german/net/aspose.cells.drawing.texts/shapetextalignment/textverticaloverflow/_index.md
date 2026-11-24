---
title: "ShapeTextAlignment.TextVerticalOverflow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeTextAlignment-Eigenschaft. Ruft den vertikalen Überlauftyp des Textfelds ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow/
---
## ShapeTextAlignment.TextVerticalOverflow property

Liest und setzt den vertikalen Überlauftyp des Textfelds.

```csharp
public TextOverflowType TextVerticalOverflow { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextVerticalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rechteckform hinzufügen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);

            // Setzen Sie Text, der vertikal überlaufen könnte
            shape.Text = "This is a long text that might overflow vertically if not clipped properly";

            // Rufen Sie die Textausrichtung ab und setzen Sie den vertikalen Überlauf auf Clip
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;

            // Speichere die Arbeitsmappe
            workbook.Save("TextVerticalOverflowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextOverflowType](../../../aspose.cells.drawing/textoverflowtype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


