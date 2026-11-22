---
title: "ShapePathPoint.XPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapePathPoint. عندما يكون الكائن إحداثيات موقع احصل على أو اضبط إحداثي x بالبكسل"
type: docs
url: /ar/net/aspose.cells.drawing/shapepathpoint/xpixel/
---
## ShapePathPoint.XPixel property

عندما يكون الكائن إحداثيًا موقعًا، احصل أو اضبط إحداثي x بالبكسل.

```csharp
public int XPixel { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXPixelDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء مجموعة نقاط مسار الشكل
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // إضافة نقاط بإحداثيات
                pathPoints.Add(100, 50);
                pathPoints.Add(200, 100);

                // الوصول إلى النقطة الأولى وإظهار خاصية XPixel
                ShapePathPoint firstPoint = pathPoints[0];

                // عرض قيمة XPixel (عملية قراءة)
                Console.WriteLine($"Initial XPixel value: {firstPoint.XPixel}");

                // تعيين قيمة جديدة لـ XPixel (نظرًا لأنها قابلة للقراءة والكتابة)
                firstPoint.XPixel = 150;
                Console.WriteLine($"Updated XPixel value: {firstPoint.XPixel}");

                // إنشاء مسار شكل وإضافة النقاط
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

                // أضف النقطة الثانية
                ShapePathPoint secondPoint = pathPoints[1];
                path.LineTo(secondPoint.XPixel, secondPoint.YPixel);
                path.Close();

                // أضف شكلاً حرًا إلى ورقة العمل
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // احفظ المصنف
                workbook.Save("XPixelDemo.xlsx");
                Console.WriteLine("XPixel property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


