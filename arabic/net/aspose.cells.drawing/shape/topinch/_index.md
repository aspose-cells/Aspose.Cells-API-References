---
title: "Shape.TopInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تمثل الإزاحة العمودية للشكل من صفه العلوي بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells.drawing/shape/topinch/
---
## Shape.TopInch property

يمثل الإزاحة العمودية للشكل من صفه العلوي، بوحدة البوصة.

```csharp
public double TopInch { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopInchDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // تعيين وإظهار خاصية TopInch
            shape.TopInch = 3;
            Console.WriteLine("Shape Top position (inches): " + shape.TopInch);

            // تعديل TopInch إذا كان يساوي 3
            if (shape.TopInch == 3)
            {
                shape.TopInch = 1;
                Console.WriteLine("Modified Shape Top position (inches): " + shape.TopInch);
            }

            // احفظ المصنف
            workbook.Save("ShapeTopInchDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


