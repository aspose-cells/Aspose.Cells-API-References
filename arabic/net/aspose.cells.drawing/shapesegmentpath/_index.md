---
title: "الفئة ShapeSegmentPath"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.ShapeSegmentPath. تمثل مسارًا جزئيًا في مسار الشكل الحر"
type: docs
url: /ar/net/aspose.cells.drawing/shapesegmentpath/
---
## ShapeSegmentPath class

يمثل مسار مقطع في مسار الشكل الحر.

```csharp
public class ShapeSegmentPath
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Points](../../aspose.cells.drawing/shapesegmentpath/points/) { get; } | يحصل على النقاط في جزء المسار |
| [Type](../../aspose.cells.drawing/shapesegmentpath/type/) { get; } | يحصل على نوع جزء المسار |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeSegmentPathDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً حرًا إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddFreeform(0, 0, 0, 0, 200, 200, new ShapePath[] { new ShapePath() });

            // احصل على مسار الهندسة للشكل
            CustomGeometry geometry = shape.Geometry as CustomGeometry;
            ShapePath shapePath = geometry.Paths[0];

            // الوصول إلى أول مسار جزئي (إن وجد)
            if (shapePath.PathSegementList.Count > 0)
            {
                ShapeSegmentPath segmentPath = shapePath.PathSegementList[0];

                // عرض خصائص ShapeSegmentPath
                Console.WriteLine("Segment Path Type: " + segmentPath.Type);
                Console.WriteLine("Number of Points: " + segmentPath.Points.Count);

                // تكرار عبر النقاط في مسار الجزء
                foreach (ShapePathPoint point in segmentPath.Points)
                {
                    Console.WriteLine($"Point coordinates: X={point.X}, Y={point.Y}");
                }
            }

            // احفظ المصنف
            workbook.Save("ShapeSegmentPathDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


