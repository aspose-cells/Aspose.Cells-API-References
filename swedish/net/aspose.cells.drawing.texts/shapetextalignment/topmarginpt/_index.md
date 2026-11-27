---
title: "ShapeTextAlignment.TopMarginPt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeTextAlignment-egenskap. Returnerar den övre marginalen i enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing.texts/shapetextalignment/topmarginpt/
---
## ShapeTextAlignment.TopMarginPt property

Returnerar den övre marginalen i enheten punkter

```csharp
public double TopMarginPt { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTopMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            shape.Text = "Sample Text";
            
            shape.TextBody.TextAlignment.TopMarginPt = 2.0d;
            
            workbook.Save("ShapeTextAlignmentTopMarginPtDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


