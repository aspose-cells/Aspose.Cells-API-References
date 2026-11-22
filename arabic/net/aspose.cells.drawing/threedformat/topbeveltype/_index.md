---
title: "ThreeDFormat.TopBevelType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreeDFormat. تحصل وتعيّن نوع الحافة العلوية أو مدى تطبيقها على الشكل. بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing/threedformat/topbeveltype/
---
## ThreeDFormat.TopBevelType property

يحصل على ويضبط نوع الحافة العلوية، أو مدى تطبيقها داخل الشكل. بوحدة النقاط.

```csharp
public BevelType TopBevelType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyTopBevelTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
            
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            workbook.Save("ThreeDFormatTopBevelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [BevelType](../../beveltype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


