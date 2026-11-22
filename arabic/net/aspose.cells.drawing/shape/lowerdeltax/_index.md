---
title: "Shape.LowerDeltaX"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل أو تعين الإزاحة الأفقية للشكل من عمود الزاوية السفلية اليمنى"
type: docs
url: /ar/net/aspose.cells.drawing/shape/lowerdeltax/
---
## Shape.LowerDeltaX property

يحصل أو يضبط الإزاحة الأفقية للشكل من عمود الزاوية السفلية اليمنى.

```csharp
public int LowerDeltaX { get; set; }
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
    public class ShapePropertyLowerDeltaXDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // تعيين وإظهار خاصية LowerDeltaX
            shape.LowerDeltaX = 3;
            Console.WriteLine("Initial LowerDeltaX: " + shape.LowerDeltaX);

            // تعديل LowerDeltaX إذا تم استيفاء الشرط
            if (shape.LowerDeltaX == 3)
            {
                shape.LowerDeltaX = 1;
                Console.WriteLine("Modified LowerDeltaX: " + shape.LowerDeltaX);
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


