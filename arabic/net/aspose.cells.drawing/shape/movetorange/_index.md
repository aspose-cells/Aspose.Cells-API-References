---
title: "Shape.MoveToRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. ينقل الشكل إلى نطاق محدد"
type: docs
url: /ar/net/aspose.cells.drawing/shape/movetorange/
---
## Shape.MoveToRange method

ينقل الشكل إلى نطاق محدد.

```csharp
public void MoveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| الصف السفلي | Int32 | فهرس الصف السفلي الأيمن |
| rightColumn | Int32 | فهرس العمود السفلي الأيمن |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodMoveToRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // انقل الشكل إلى نطاق محدد
            shape.MoveToRange(12, 3, 13, 5);

            // احفظ المصنف
            workbook.Save("ShapeMoveToRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


