---
title: "ThreeDFormat.RotationZ"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreeDFormat. يحصل على ويضبط دوران الشكل المستخرج حول المحور z بالدرجات"
type: docs
url: /ar/net/aspose.cells.drawing/threedformat/rotationz/
---
## ThreeDFormat.RotationZ property

يحصل ويضبط دوران الشكل المُبثق حول المحور z بالدرجات.

```csharp
public double RotationZ { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationZDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل لتوضيح تنسيق ثلاثي الأبعاد
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 0, 100, 150);
            shape.Text = "3D Rotation Demo";
            
            // الوصول إلى ThreeDFormat الخاص بالشكل
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // عرض قيمة RotationZ الحالية
            Console.WriteLine("Current RotationZ value: " + threeDFormat.RotationZ);

            // تعيين قيم RotationZ جديدة وإظهار التأثيرات
            threeDFormat.RotationZ = 45;
            Console.WriteLine("Shape rotated 45 degrees around Z-axis");

            // تطبيق خصائص ثلاثية الأبعاد أخرى لجعل الدوران مرئيًا
            threeDFormat.ExtrusionHeight = 15;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;

            // حفظ المصنف مع تأثيرات ثلاثية الأبعاد
            workbook.Save("ThreeDFormatRotationZDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


