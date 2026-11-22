---
title: "Shape.AlignTopRightCorner"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. تنقل الصورة إلى الزاوية العليا اليمنى"
type: docs
url: /ar/net/aspose.cells.drawing/shape/aligntoprightcorner/
---
## Shape.AlignTopRightCorner method

ينقل الصورة إلى الزاوية العليا اليمنى.

```csharp
public void AlignTopRightCorner(int topRow, int rightColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف. |
| rightColumn | Int32 | فهرس العمود. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodAlignTopRightCornerWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً نموذجيًا للمحاذاة
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // حاذِ الزاوية العليا اليمنى للشكل إلى الصف 2، العمود 5
            shape.AlignTopRightCorner(2, 5);

            // احفظ المصنف
            workbook.Save("AlignTopRightCornerDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


