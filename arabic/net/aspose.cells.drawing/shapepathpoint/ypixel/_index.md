---
title: "ShapePathPoint.YPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapePathPoint. عندما يكون الكائن إحداثيًا موضعًا، احصل أو اضبط إحداثي y بالبكسل"
type: docs
url: /ar/net/aspose.cells.drawing/shapepathpoint/ypixel/
---
## ShapePathPoint.YPixel property

عندما يكون الكائن إحداثيًا موقعًا، احصل أو اضبط إحداثي y بالبكسل.

```csharp
public int YPixel { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYPixelDemo
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

                // إضافة نقطة مع الإحداثيات
                pathPoints.Add(100, 50);

                // الوصول إلى النقطة الأولى وعرض خاصية YPixel
                ShapePathPoint firstPoint = pathPoints[0];

                // عرض قيمة YPixel الأولية (عملية قراءة)
                Console.WriteLine($"Initial YPixel value: {firstPoint.YPixel}");

                // تعيين قيمة جديدة لـ YPixel (نظرًا لأنه قابل للقراءة/الكتابة)
                firstPoint.YPixel = 150;
                Console.WriteLine($"Updated YPixel value: {firstPoint.YPixel}");

                // إنشاء مسار شكل واستخدام النقطة
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

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
                workbook.Save("YPixelDemo.xlsx");
                Console.WriteLine("YPixel property demonstration completed successfully.");
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


