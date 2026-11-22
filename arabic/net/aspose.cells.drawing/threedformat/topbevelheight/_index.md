---
title: "ThreeDFormat.TopBevelHeight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreeDFormat. يسترجع ويعيّن ارتفاع الحافة العلوية أو مدى تطبيقها داخل الشكل. بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing/threedformat/topbevelheight/
---
## ThreeDFormat.TopBevelHeight property

يحصل ويضبط ارتفاع الحافة العلوية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط.

```csharp
public double TopBevelHeight { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyTopBevelHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
            
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.TopBevelType = BevelType.Circle;
            threeDFormat.TopBevelHeight = 15;
            threeDFormat.TopBevelWidth = 10;

            workbook.Save("ThreeDFormatTopBevelHeightDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


