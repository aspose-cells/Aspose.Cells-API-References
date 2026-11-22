---
title: "Shape.WidthInShape"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الشكل. تمثل عرض الشكل بوحدة 1/4000 من الشكل الأب"
type: docs
url: /ar/net/aspose.cells.drawing/shape/widthinshape/
---
## Shape.WidthInShape property

يمثل عرض الشكل، بوحدة 1/4000 من الشكل الأب.

```csharp
public int WidthInShape { get; set; }
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
    public class ShapePropertyWidthInShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أنشئ شكلين مستطيلين
            Shape rect1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            Shape rect2 = worksheet.Shapes.AddRectangle(0, 100, 0, 0, 100, 100);
            
            // تجميع الأشكال باستخدام كائنات الشكل
            GroupShape group = worksheet.Shapes.Group(new Shape[] { rect1, rect2 });
            
            // عرض مثال لاستخدام WidthInShape
            if (rect1.IsInGroup && rect1.WidthInShape == 2000)
            {
                rect1.WidthInShape = 4000;
            }
            
            // حفظ المصنف المعدل
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


