---
title: "Shape.UpperDeltaX"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. يحصل على أو يضبط الإزاحة الأفقية للشكل من عمود الزاوية العلوية اليسرى"
type: docs
url: /ar/net/aspose.cells.drawing/shape/upperdeltax/
---
## Shape.UpperDeltaX property

يحصل أو يضبط الإزاحة الأفقية للشكل من عمود الزاوية العلوية اليسرى.

```csharp
public int UpperDeltaX { get; set; }
```

### ملاحظات

نطاق القيمة هو من 0 إلى 1024.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperDeltaXDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // اضبط واعرض خاصية UpperDeltaX
            shape.UpperDeltaX = 150;
            Console.WriteLine("UpperDeltaX: " + shape.UpperDeltaX);

            // عدّل UpperDeltaX إذا استوفى شرطًا
            if (shape.UpperDeltaX == 150)
            {
                shape.UpperDeltaX = 100;
                Console.WriteLine("Modified UpperDeltaX: " + shape.UpperDeltaX);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


