---
title: "Shape.UpperLeftRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل فهرس الصف العلوي"
type: docs
url: /ar/net/aspose.cells.drawing/shape/upperleftrow/
---
## Shape.UpperLeftRow property

يمثل فهرس الصف العلوي.

```csharp
public int UpperLeftRow { get; set; }
```

### ملاحظات

إذا كان الشكل داخل الشكل أو داخل المجموعة، سيتم تجاهل UpperLeftRow.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyUpperLeftRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // تعيين وعرض خاصية UpperLeftRow
            shape.UpperLeftRow = 3;
            Console.WriteLine("Shape's initial topRow: " + shape.UpperLeftRow);

            // تعديل UpperLeftRow بناءً على الشرط
            if (shape.UpperLeftRow == 3)
                shape.UpperLeftRow = 1;

            Console.WriteLine("Shape's modified topRow: " + shape.UpperLeftRow);
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


