---
title: "ThreeDFormat.Perspective"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreeDFormat. تحصل وتضبط الزاوية التي يمكن رؤية كائن ThreeDFormat عندها"
type: docs
url: /ar/net/aspose.cells.drawing/threedformat/perspective/
---
## ThreeDFormat.Perspective property

يحصل ويضبط الزاوية التي يمكن من خلالها عرض كائن ThreeDFormat.

```csharp
public double Perspective { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyPerspectiveDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل لتوضيح تنسيق ثلاثي الأبعاد
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 0, 0, 200, 100);
            
            // احصل على تنسيق ثلاثي الأبعاد للشكل
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // اعرض القيمة الحالية للمنظور
            Console.WriteLine("Current Perspective value: " + threeDFormat.Perspective);

            // اضبط قيمة منظور جديدة (0 إلى 120 درجة)
            threeDFormat.Perspective = 45;
            Console.WriteLine("Perspective set to: " + threeDFormat.Perspective);

            // طبق تأثيرات ثلاثية الأبعاد أخرى لتصور تغيير المنظور بشكل أفضل
            threeDFormat.ExtrusionHeight = 15;
            threeDFormat.ContourWidth = 2;
            threeDFormat.RotationX = 20;
            threeDFormat.RotationY = 30;

            // حفظ المصنف لرؤية التأثيرات
            workbook.Save("ThreeDFormatPerspectiveDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


