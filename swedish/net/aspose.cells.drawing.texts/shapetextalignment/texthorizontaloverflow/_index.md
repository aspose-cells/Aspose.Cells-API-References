---
title: "ShapeTextAlignment.TextHorizontalOverflow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeTextAlignment-egenskap. Hämtar och anger typ av horisontell översvämning för textrutan"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow/
---
## ShapeTextAlignment.TextHorizontalOverflow property

Hämtar och anger den horisontella översvämningstypen för texten i textrutan.

```csharp
public TextOverflowType TextHorizontalOverflow { get; set; }
```

### Exempel

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

            // Lägg till en textruta
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 50);
            textBox.Text = "This is a long text that demonstrates horizontal overflow behavior";

            // Ställ in horisontell översvämning till Clip
            textBox.TextBody.TextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;

            // Spara arbetsboken
            workbook.Save("TextHorizontalOverflowDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextOverflowType](../../../aspose.cells.drawing/textoverflowtype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


