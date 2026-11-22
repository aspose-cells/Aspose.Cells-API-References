---
title: "ThreeDFormat.RotationX"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreeDFormat. يحصل على ويضبط دوران الشكل المستخرج حول المحور x بالدرجات"
type: docs
url: /ar/net/aspose.cells.drawing/threedformat/rotationx/
---
## ThreeDFormat.RotationX property

يحصل ويضبط دوران الشكل المُبثق حول المحور x بالدرجات.

```csharp
public double RotationX { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationXDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل لتوضيح تنسيق ثلاثي الأبعاد
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 2, 2, 200, 100, 100);
            
            // احصل على تنسيق ثلاثي الأبعاد (ليس هناك حاجة \"لتفعيل\" تأثيرات ثلاثية الأبعاد - فقط اضبط الخصائص)
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // عرض قيمة RotationX الحالية
            Console.WriteLine("Current RotationX value: " + threeDFormat.RotationX);

            // تعيين قيمة RotationX جديدة (الدوران حول المحور x بالدرجات)
            threeDFormat.RotationX = 45;
            Console.WriteLine("New RotationX value: " + threeDFormat.RotationX);

            // تعيين خصائص ثلاثية الأبعاد أخرى لجعل الدوران مرئيًا
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;

            // حفظ المصنف لرؤية التأثيرات
            workbook.Save("ThreeDFormatRotationXDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


