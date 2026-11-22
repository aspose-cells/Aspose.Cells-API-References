---
title: "ThreeDFormat.ContourWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreeDFormat. تحصل وتضبط عرض الحد على الشكل بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing/threedformat/contourwidth/
---
## ThreeDFormat.ContourWidth property

يحصل ويضبط عرض الخط المحيط على الشكل، بوحدة النقاط.

```csharp
public double ContourWidth { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyContourWidthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // أضف شكلاً إلى ورقة العمل مع جميع المعلمات المطلوبة
            Shape sh = ws.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);

            // تطبيق تنسيق 3D
            ThreeDFormat n3df = sh.ThreeDFormat;
            n3df.ContourWidth = 17;
            n3df.ExtrusionHeight = 32;
            n3df.TopBevelType = (BevelType)BevelPresetType.HardEdge;

            // احفظ المصنف
            wb.Save("output.xlsx");

            // تحقق من القيم المحفوظة
            Workbook wb2 = new Workbook("output.xlsx");
            Shape sh2 = wb2.Worksheets[0].Shapes[0];
            ThreeDFormat n3df2 = sh2.ThreeDFormat;

            Console.WriteLine("ContourWidth: " + n3df2.ContourWidth);
            Console.WriteLine("ExtrusionHeight: " + n3df2.ExtrusionHeight);
            Console.WriteLine("TopBevelType: " + n3df2.TopBevelType);
        }
    }
}
```

### انظر أيضًا

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


