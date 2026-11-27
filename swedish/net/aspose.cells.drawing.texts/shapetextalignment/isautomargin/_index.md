---
title: "ShapeTextAlignment.IsAutoMargin"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeTextAlignment-egenskapen. Anger om marginalen för textramen är automatisk"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextalignment/isautomargin/
---
## ShapeTextAlignment.IsAutoMargin property

Anger om marginalen för textramen är automatisk.

```csharp
public bool IsAutoMargin { get; set; }
```

### Exempel

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

            // Lägg till en rektangel med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Kom åt textjustering och ställ in IsAutoMargin
            shape.TextBody.TextAlignment.IsAutoMargin = true;

            // Ställ in lite text för att demonstrera
            shape.Text = "Sample text with auto margins";

            // Spara arbetsboken
            workbook.Save("ShapeTextAlignmentIsAutoMarginDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


