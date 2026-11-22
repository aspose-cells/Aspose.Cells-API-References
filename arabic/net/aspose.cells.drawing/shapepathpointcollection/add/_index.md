---
title: "ShapePathPointCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapePathPointCollection. تُضيف نقطة مسار بوحدة EMUs"
type: docs
url: /ar/net/aspose.cells.drawing/shapepathpointcollection/add/
---
## ShapePathPointCollection.Add method

تضيف نقطة مسار بوحدة EMUs.

```csharp
[Obsolete("Use the MoveTo,LineTo,CubicBezierTo and ArcTo methods in ShapePath instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int x, int y)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| x | Int32 | الإحداثي x. |
| y | Int32 | الإحداثي y. |

### ملاحظات

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام طرق MoveTo وLineTo وCubicBezierTo وArcTo في ShapePath. سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من أغسطس 2025. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مجموعة نقاط مسار الشكل
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();

            try
            {
                // استدعِ طريقة Add مع معلمات (Int32, Int32)
                pathPoints.Add(50, 10);
                pathPoints.Add(50, 50);
                pathPoints.Add(10, 50);

                // إنشاء مسار شكل وإضافة النقاط
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

                // حفظ النتيجة
                workbook.Save("ShapePathPointCollectionMethodAddWithInt32Int32Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ShapePathPointCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


