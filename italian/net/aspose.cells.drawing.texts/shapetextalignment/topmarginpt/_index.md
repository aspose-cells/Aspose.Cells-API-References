---
title: "ShapeTextAlignment.TopMarginPt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapeTextAlignment. Restituisce il margine superiore in unità di punti"
type: docs
url: /it/net/aspose.cells.drawing.texts/shapetextalignment/topmarginpt/
---
## ShapeTextAlignment.TopMarginPt property

Restituisce il margine superiore in unità di punti

```csharp
public double TopMarginPt { get; set; }
```

### Esempi

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

### Vedi anche

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


