---
title: "Shape.Top"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الشكل. تمثل الإزاحة الرأسية للشكل عن صفه العلوي بوحدة البكسل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/top/
---
## Shape.Top property

يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البكسل.

```csharp
public int Top { get; set; }
```

### ملاحظات

إذا كان الشكل في المخطط، تمثّل الإزاحة العمودية للشكل من حدّه العلوي

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // تعيين الموضع العلوي الأولي
            shape.Top = 50;
            Console.WriteLine("Initial Top position: " + shape.Top);

            // تعديل الموضع العلوي إذا كان يساوي 3 (لتوضيح منطق حالة الاختبار)
            if (shape.Top == 3)
            {
                shape.Top = 1;
            }
            else
            {
                // للتوضيح، اضبطه إلى 3 ثم طبق منطق حالة الاختبار
                shape.Top = 3;
                if (shape.Top == 3)
                {
                    shape.Top = 1;
                    Console.WriteLine("Modified Top position: " + shape.Top);
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


