---
title: "ShapeTextAlignment.LeftMarginPt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeTextAlignment-egenskapen. Returnerar den vänstra marginalen i enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextalignment/leftmarginpt/
---
## ShapeTextAlignment.LeftMarginPt property

Returnerar den vänstra marginalen i enheten punkter

```csharp
public double LeftMarginPt { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangel med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            
            // Ange text för formen
            shape.Text = "Sample text with left margin";

            // Kom åt textjustering och ställ in vänster marginal i punkter
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            textAlignment.LeftMarginPt = 2.0d;

            // Spara arbetsboken
            workbook.Save("ShapeTextAlignmentLeftMarginPtDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


