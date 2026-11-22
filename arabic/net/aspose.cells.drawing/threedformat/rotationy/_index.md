---
title: "ThreeDFormat.RotationY"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreeDFormat. تحصل وتعيّن دوران الشكل المستخرج حول المحور y بالدرجات"
type: docs
url: /ar/net/aspose.cells.drawing/threedformat/rotationy/
---
## ThreeDFormat.RotationY property

يحصل ويضبط دوران الشكل المُبثق حول المحور y بالدرجات.

```csharp
public double RotationY { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationYDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل لتوضيح تنسيق ثلاثي الأبعاد
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 100, 150, 150);
            shape.Text = "3D Rotation Demo";
            
            // الوصول إلى ThreeDFormat الخاص بالشكل
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // عرض قيمة RotationY الحالية
            Console.WriteLine("Current RotationY value: " + threeDFormat.RotationY);

            // تعيين قيم RotationY جديدة وإظهار التأثيرات
            threeDFormat.RotationY = 15;
            Console.WriteLine("Shape rotated 15 degrees around Y-axis");

            // تطبيق بعض الخصائص الثلاثية الأبعاد الأخرى لجعل التأثير مرئياً
            threeDFormat.ExtrusionHeight = 5;
            threeDFormat.ContourWidth = 1;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;

            // حفظ المصنف لإظهار التأثيرات
            workbook.Save("ThreeDFormatRotationYDemo.xlsx");

            // تغيير الدوران مرة أخرى وحفظ نسخة أخرى
            threeDFormat.RotationY = 45;
            workbook.Save("ThreeDFormatRotationYDemo_45degrees.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


