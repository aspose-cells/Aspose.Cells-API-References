---
title: "ShapeTextAlignment.TextHorizontalOverflow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapeTextAlignment Eigenschaft. Liest und setzt den horizontalen Überlauftyp des Textfelds"
type: docs
url: /de/net/aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow/
---
## ShapeTextAlignment.TextHorizontalOverflow property

Liest und setzt den horizontalen Überlauftyp des Textfelds.

```csharp
public TextOverflowType TextHorizontalOverflow { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextHorizontalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie eine Textfeldform hinzu
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 50);
            textBox.Text = "This is a long text that demonstrates horizontal overflow behavior";

            // Setze den horizontalen Überlauf auf Clip
            textBox.TextBody.TextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;

            // Speichere die Arbeitsmappe
            workbook.Save("TextHorizontalOverflowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TextOverflowType](../../../aspose.cells.drawing/textoverflowtype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


