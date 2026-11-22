---
title: "ShapePathPoint.X"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapePathPoint. يحصل على ويضبط إحداثي x لهذا الإحداثي الموضع. الوحدة EMUs"
type: docs
url: /ar/net/aspose.cells.drawing/shapepathpoint/x/
---
## ShapePathPoint.X property

يحصل على ويضبط إحداثي x لهذا الإحداثي الموضع. الوحدة EMUs.

```csharp
[Obsolete("Use ShapePathPoint.XPixel and ShapePathPoint.XAngle properties instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int X { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام خصائص ShapePathPoint.XPixel و ShapePathPoint.XAngle. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من أغسطس 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مجموعة نقاط مسار الشكل وإضافة نقاط
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(50, 10);
            pathPoints.Add(50, 50);
            pathPoints.Add(10, 50);

            // الوصول إلى النقاط باستخدام خاصية Item
            Console.WriteLine("First point coordinates:");
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"X: {firstPoint.X}, Y: {firstPoint.Y}");

            Console.WriteLine("\nAll points in collection:");
            for (int i = 0; i < pathPoints.Count; i++)
            {
                ShapePathPoint point = pathPoints[i];
                Console.WriteLine($"Point {i}: X={point.X}, Y={point.Y}");
            }

            // إنشاء مسار شكل باستخدام النقاط
            ShapePath path = new ShapePath();

            // الانتقال إلى النقطة البداية
            path.MoveTo(10, 10);

            foreach (ShapePathPoint point in pathPoints)
            {
                path.LineTo(point.X, point.Y);
            }
            path.Close();

            // إضافة شكل حر مع المسار المُكوَّن
            Shape shape = worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path }
                );

            // حفظ المصنف المعدل
            workbook.Save("ShapePathPointXDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


