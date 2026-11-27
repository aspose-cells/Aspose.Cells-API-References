---
title: "ShapeTextAlignment.RightMarginPt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeTextAlignment-egenskap. Returnerar högermarginalen i enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextalignment/rightmarginpt/
---
## ShapeTextAlignment.RightMarginPt property

Returnerar den högra marginalen i enheten punkter

```csharp
public double RightMarginPt { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangel med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Åtkomst till textjusteringen
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // Ange högermarginalen i punkter
            shapeTextAlignment.RightMarginPt = 2.0d;

            // Verifiera egenskapen genom att hämta tillbaka värdet
            Console.WriteLine("Right Margin in Points: " + shapeTextAlignment.RightMarginPt);
        }
    }
}
```

### Se även

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


