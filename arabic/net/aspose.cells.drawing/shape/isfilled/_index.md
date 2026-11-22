---
title: "Shape.IsFilled"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تشير إلى ما إذا كان تنسيق التعبئة مرئيًا"
type: docs
url: /ar/net/aspose.cells.drawing/shape/isfilled/
---
## Shape.IsFilled property

يشير إلى ما إذا كان تنسيق التعبئة مرئيًا.

```csharp
public bool IsFilled { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsFilledDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // تحقق وعدّل خاصية IsFilled
            if (shape.IsFilled == false)
            {
                shape.IsFilled = true;
                shape.FillFormat.ForeColor = System.Drawing.Color.Red;
            }

            // احفظ المصنف
            workbook.Save("ShapeIsFilledDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


