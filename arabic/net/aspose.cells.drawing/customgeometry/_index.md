---
title: "الفئة CustomGeometry"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.CustomGeometry. تمثل شكلاً هندسياً مخصصاً"
type: docs
url: /ar/net/aspose.cells.drawing/customgeometry/
---
## CustomGeometry class

يمثل شكلاً هندسياً مخصصاً.

```csharp
public class CustomGeometry : Geometry
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Paths](../../aspose.cells.drawing/customgeometry/paths/) { get; } | الحصول على معلومات مجموعة المسارات عندما يكون الشكل NotPrimitive autoshape |
| [ShapeAdjustValues](../../aspose.cells.drawing/geometry/shapeadjustvalues/) { get; } | الحصول على مجموعة من قيم تعديل الشكل (مستمدة من [`Geometry`](../geometry/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassCustomGeometryDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة NotPrimitive autoshape مع المعلمات الصحيحة
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 0, 0, 200, 300);

            // الحصول على مثيل CustomGeometry من الشكل
            CustomGeometry customGeometry = shape.Geometry as CustomGeometry;

            // إنشاء مسار جديد في مجموعة مسارات الهندسة
            int pathIndex = customGeometry.Paths.Add();
            ShapePath path = customGeometry.Paths[pathIndex];

            // إضافة مقاطع مسار باستخدام استدعاءات طريقة مباشرة
            path.MoveTo(0, 0);
            path.LineTo(1000, 0);
            path.LineTo(1000, 1000);
            path.LineTo(0, 1000);
            path.Close();

            // احفظ المصنف
            workbook.Save("CustomGeometryDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Geometry](../geometry/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


