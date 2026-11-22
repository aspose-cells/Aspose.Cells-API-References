---
title: "CustomGeometry.Paths"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CustomGeometry. يحصل على معلومات مجموعة المسارات عندما يكون الشكل NotPrimitive autoshape"
type: docs
url: /ar/net/aspose.cells.drawing/customgeometry/paths/
---
## CustomGeometry.Paths property

الحصول على معلومات مجموعة المسارات عندما يكون الشكل NotPrimitive autoshape

```csharp
public ShapePathCollection Paths { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CustomGeometryPropertyPathsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مخصص مع هندسة غير بدائية (معلمات ثابتة)
            var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.NotPrimitive, 0, 0, 10, 10, 400, 400);
            
            // الوصول إلى الهندسة المخصصة عبر التحويل الصريح
            CustomGeometry geometry = (CustomGeometry)shape.Geometry;
            
            // الحصول على مجموعة المسارات
            ShapePathCollection paths = geometry.Paths;
            Console.WriteLine($"Initial path count: {paths.Count}");

            // إنشاء مسار شكل جديد باستخدام أوامر الرسم
            paths.Add(); // Creates a new path in the collection
            ShapePath newPath = paths[paths.Count - 1];
            newPath.MoveTo(0, 0);
            newPath.LineTo(10000, 0);
            newPath.LineTo(10000, 10000);
            newPath.LineTo(0, 10000);
            newPath.Close();

            // لا حاجة إلى إضافة صريحة لأن المسار تم إنشاؤه في المجموعة
            Console.WriteLine($"New path count after modification: {paths.Count}");

            // احفظ لتوضيح التغييرات الدائمة
            workbook.Save("CustomGeometryPathsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapePathCollection](../../shapepathcollection/)
* class [CustomGeometry](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


