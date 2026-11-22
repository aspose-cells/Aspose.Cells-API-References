---
title: "Shape.HeightInShape"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل الإزاحة العمودية للشكل من الحد العلوي للشكل الأب بوحدة 1/4000 من ارتفاع الشكل الأب"
type: docs
url: /ar/net/aspose.cells.drawing/shape/heightinshape/
---
## Shape.HeightInShape property

يمثل الإزاحة العمودية للشكل من الحد العلوي للشكل الأب، بوحدة 1/4000 من ارتفاع الشكل الأب..

```csharp
public int HeightInShape { get; set; }
```

### ملاحظات

يطبق فقط عندما يكون هذا الشكل داخل مجموعة أو مخطط.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightInShapeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف الأشكال أولاً مع جميع المعلمات المطلوبة
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 10, 10);
            Shape oval = worksheet.Shapes.AddOval(0, 0, 100, 100, 10, 120);

            // اجمع الأشكال
            Shape[] shapes = { rectangle, oval };
            GroupShape groupShape = worksheet.Shapes.Group(shapes);

            // اضبط ارتفاع المستطيل نسبةً إلى شكل المجموعة الأصل (1/4000 من ارتفاع الأصل)
            rectangle.HeightInShape = 2000; // Half the height of the parent
            oval.HeightInShape = 4000; // Full height of the parent

            // احفظ المصنف
            workbook.Save("ShapeHeightInShapeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


