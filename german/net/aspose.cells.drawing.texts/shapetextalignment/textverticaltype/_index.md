---
title: "ShapeTextAlignment.TextVerticalType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeTextAlignment Eigenschaft. Liest und setzt die Textrichtung"
type: docs
url: /de/net/aspose.cells.drawing.texts/shapetextalignment/textverticaltype/
---
## ShapeTextAlignment.TextVerticalType property

Liest und setzt die Textausrichtung.

```csharp
public TextVerticalType TextVerticalType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextVerticalTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Textfeld-Form mit korrekten Parametern hinzu
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            shape.Text = "Sample Text";

            // Textausrichtung abrufen und vertikalen Texttyp festlegen
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            textAlignment.TextVerticalType = TextVerticalType.Horizontal;

            // Speichere die Arbeitsmappe
            workbook.Save("TextVerticalTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextVerticalType](../../textverticaltype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


