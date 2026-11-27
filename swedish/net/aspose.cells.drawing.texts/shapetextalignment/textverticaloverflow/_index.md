---
title: "ShapeTextAlignment.TextVerticalOverflow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeTextAlignment-egenskapen. Hämtar och anger den vertikala översvämningstypen för textrutan"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow/
---
## ShapeTextAlignment.TextVerticalOverflow property

Hämtar och anger den vertikala översvämningstypen för texten i textrutan.

```csharp
public TextOverflowType TextVerticalOverflow { get; set; }
```

### Exempel

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

            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);

            // Ställ in text som kan flöda över vertikalt
            shape.Text = "This is a long text that might overflow vertically if not clipped properly";

            // Hämta textjustering och ställ in vertikal översvämning till Clip
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;

            // Spara arbetsboken
            workbook.Save("TextVerticalOverflowDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextOverflowType](../../../aspose.cells.drawing/textoverflowtype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


