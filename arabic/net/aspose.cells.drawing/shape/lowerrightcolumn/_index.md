---
title: "Shape.LowerRightColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل فهرس عمود الزاوية السفلية اليمنى"
type: docs
url: /ar/net/aspose.cells.drawing/shape/lowerrightcolumn/
---
## Shape.LowerRightColumn property

يمثل فهرس العمود للزاوية السفلية اليمنى.

```csharp
public int LowerRightColumn { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLowerRightColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلًا إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // قم بتعيين وعرض القيمة الأولية لـ LowerRightColumn
            shape.LowerRightColumn = 3;
            Console.WriteLine("Initial LowerRightColumn: " + shape.LowerRightColumn);

            // عدّل LowerRightColumn إذا كان يساوي 3
            if (shape.LowerRightColumn == 3)
            {
                shape.LowerRightColumn = 1;
                Console.WriteLine("Modified LowerRightColumn: " + shape.LowerRightColumn);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


