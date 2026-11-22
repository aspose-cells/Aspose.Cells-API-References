---
title: "Shape.IsInGroup"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الشكل. تشير إلى ما إذا كان الشكل ضمن مجموعة"
type: docs
url: /ar/net/aspose.cells.drawing/shape/isingroup/
---
## Shape.IsInGroup property

يشير إلى ما إذا كان الشكل مجموعة.

```csharp
public bool IsInGroup { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyIsInGroupDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض الأشكال مع جميع المعلمات المطلوبة (upperLeftRow, upperLeftColumn, height, width, imageWidth, imageHeight)
            Shape shape1 = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 50, 100);
            Shape shape2 = worksheet.Shapes.AddRectangle(6, 0, 2, 0, 50, 100);
            Shape shape3 = worksheet.Shapes.AddRectangle(3, 0, 5, 0, 50, 100);

            // تجميع الأشكال مع المعلمات الصحيحة
            GroupShape group = worksheet.Shapes.Group(new Shape[] { shape1, shape2, shape3 });

            // التحقق مما إذا كانت الأشكال ضمن مجموعة
            Console.WriteLine("Shape1 IsInGroup: " + shape1.IsInGroup);
            Console.WriteLine("Shape2 IsInGroup: " + shape2.IsInGroup);
            Console.WriteLine("Shape3 IsInGroup: " + shape3.IsInGroup);
            Console.WriteLine("GroupShape IsInGroup: " + group.IsInGroup);

            // إضافة شكل غير مجمّع
            Shape ungroupedShape = worksheet.Shapes.AddRectangle(10, 0, 2, 0, 50, 100);
            Console.WriteLine("Ungrouped shape IsInGroup: " + ungroupedShape.IsInGroup);

            // حفظ النتيجة
            workbook.Save("ShapePropertyIsInGroupDemo.xlsx");

            // فك تجميع الأشكال والحصول على الأشكال غير المجمّعة من المجموعة
            group.Ungroup();
            Console.WriteLine("After ungrouping, shape1 IsInGroup: " + shape1.IsInGroup);
            Console.WriteLine("After ungrouping, shape2 IsInGroup: " + shape2.IsInGroup);
            Console.WriteLine("After ungrouping, shape3 IsInGroup: " + shape3.IsInGroup);

            // حفظ النتيجة
            workbook.Save("ShapePropertyIsInGroupDemo2.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


