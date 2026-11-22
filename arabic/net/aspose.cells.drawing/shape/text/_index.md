---
title: "Shape.Text"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. يحصل على ويضبط نص هذا الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/text/
---
## Shape.Text property

يحصل ويضبط نص هذا الشكل.

```csharp
public string Text { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلًا مستطيلًا بالمعلمات الصحيحة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // اضبط النص إذا كان فارغًا
            if (shape.Text == null)
            {
                shape.Text = "This is a test.";
            }

            // عدّل النص
            shape.Text = "Updated text demo";

            // احفظ المصنف
            workbook.Save("ShapeTextDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


