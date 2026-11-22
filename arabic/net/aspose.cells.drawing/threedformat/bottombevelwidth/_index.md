---
title: "ThreeDFormat.BottomBevelWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreeDFormat. تحصل وتضبط عرض الحافة السفلية أو مدى تطبيقها داخل الشكل. بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing/threedformat/bottombevelwidth/
---
## ThreeDFormat.BottomBevelWidth property

يحصل ويضبط عرض الحافة السفلية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط.

```csharp
public double BottomBevelWidth { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyBottomBevelWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            threeDFormat.BottomBevelType = BevelType.ArtDeco;
            threeDFormat.BottomBevelWidth = 15;
            threeDFormat.BottomBevelHeight = 8;

            workbook.Save("ThreeDFormatBottomBevelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


