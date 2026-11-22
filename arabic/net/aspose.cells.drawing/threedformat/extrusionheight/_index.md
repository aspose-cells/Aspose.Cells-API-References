---
title: "ThreeDFormat.ExtrusionHeight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreeDFormat. تحصل وتضبط ارتفاع البثق المطبق على الشكل بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing/threedformat/extrusionheight/
---
## ThreeDFormat.ExtrusionHeight property

يحصل ويضبط ارتفاع البثق المطبق على الشكل، بوحدة النقاط.

```csharp
public double ExtrusionHeight { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyExtrusionHeightDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا نموذجيًا مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // تطبيق تنسيق 3D
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.ExtrusionHeight = 32;
            threeDFormat.ContourWidth = 17;
            threeDFormat.TopBevelType = BevelType.HardEdge;
            threeDFormat.TopBevelWidth = 30;
            threeDFormat.TopBevelHeight = 30;

            // احفظ المصنف
            workbook.Save("output.xlsx");

            // تحقق من القيم المحفوظة
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ThreeDFormat loadedFormat = loadedShape.ThreeDFormat;

            Console.WriteLine("ExtrusionHeight: " + loadedFormat.ExtrusionHeight);
            Console.WriteLine("ContourWidth: " + loadedFormat.ContourWidth);
            Console.WriteLine("TopBevelType: " + loadedFormat.TopBevelType);
            Console.WriteLine("TopBevelWidth: " + loadedFormat.TopBevelWidth);
            Console.WriteLine("TopBevelHeight: " + loadedFormat.TopBevelHeight);
        }
    }
}
```

### انظر أيضًا

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


