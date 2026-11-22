---
title: "تعداد ShapePathType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.ShapePathType. يمثل نوع مقطع المسار"
type: docs
url: /ar/net/aspose.cells.drawing/shapepathtype/
---
## ShapePathType enumeration

يمثل نوع مقطع المسار.

```csharp
public enum ShapePathType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| LineTo | `1` | مقطع خط مستقيم |
| CubicBezierCurveTo | `3` | منحنى بيزيه مكعب |
| MoveTo | `0` | ابدأ مسارًا جديدًا |
| Close | `128` | إذا لم تكن النقطة الابتدائية POINT والنقطة النهائية POINT متطابقتين، يتم رسم خط مستقيم واحد لربط النقطة الابتدائية POINT والنقطة النهائية POINT للمسار. |
| End | `4` | نهاية المسار الحالي |
| Escape | `5` | هروب |
| ArcTo | `6` | قوس |
| Unknown | `7` | غير معروف |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إنشاء شكل لعرض أنواع المسارات
                Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 10, 10, 10, 10, 200, 200);

                // إنشاء مسار هندسي مخصص
                Geometry geometry = shape.Geometry;
                ShapePath path = new ShapePath();

                // عرض قيم ShapePathType المختلفة
                Console.WriteLine("Available ShapePathType values:");
                Console.WriteLine($"LineTo: {ShapePathType.LineTo}");
                Console.WriteLine($"CubicBezierCurveTo: {ShapePathType.CubicBezierCurveTo}");
                Console.WriteLine($"MoveTo: {ShapePathType.MoveTo}");
                Console.WriteLine($"Close: {ShapePathType.Close}");
                Console.WriteLine($"End: {ShapePathType.End}");

                // تطبيق بعض عمليات المسار
                path.MoveTo(10, 10);
                path.LineTo(100, 100);
                path.Close();

                // احفظ المصنف
                workbook.Save("ShapePathTypeDemo.xlsx");
                Console.WriteLine("Demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathType: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


