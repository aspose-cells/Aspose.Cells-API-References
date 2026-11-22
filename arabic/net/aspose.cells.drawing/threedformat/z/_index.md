---
title: "ThreeDFormat.Z"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreeDFormat. تحدد المسافة من الأرض للشكل ثلاثي الأبعاد"
type: docs
url: /ar/net/aspose.cells.drawing/threedformat/z/
---
## ThreeDFormat.Z property

يحدد المسافة من الأرض للشكل ثلاثي الأبعاد.

```csharp
public double Z { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyZDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل لتوضيح تنسيق ثلاثي الأبعاد
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 0, 0, 200, 100);
            
            // الوصول إلى ThreeDFormat الخاص بالشكل
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // عرض قيمة Z الحالية (المسافة من الأرض)
            Console.WriteLine("Current Z value: " + threeDFormat.Z);

            // تعيين قيمة Z جديدة لتحريك الشكل بعيدًا عن الأرض
            threeDFormat.Z = 20;
            Console.WriteLine("New Z value: " + threeDFormat.Z);

            // تكوين خصائص ثلاثية الأبعاد أخرى لجعل التأثير مرئيًا
            threeDFormat.ExtrusionHeight = 30;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;

            // حفظ المصنف لرؤية التأثير ثلاثي الأبعاد
            workbook.Save("ThreeDFormatPropertyZDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


