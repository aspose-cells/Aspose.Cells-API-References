---
title: "ShapeTextAlignment.BottomMarginPt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapeTextAlignment. تُرجع الهامش السفلي بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing.texts/shapetextalignment/bottommarginpt/
---
## ShapeTextAlignment.BottomMarginPt property

يعيد الهامش السفلي بوحدة النقاط

```csharp
public double BottomMarginPt { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyBottomMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "Sample Text";
            
            shape.TextBody.TextAlignment.BottomMarginPt = 2.0d;
            
            Console.WriteLine("Bottom margin set to: " + shape.TextBody.TextAlignment.BottomMarginPt + " points");
        }
    }
}
```

### انظر أيضًا

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


