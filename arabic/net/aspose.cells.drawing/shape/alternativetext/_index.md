---
title: "Shape.AlternativeText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تُرجع أو تُعيّن سلسلة النص البديلة الوصفية لكائن Shape"
type: docs
url: /ar/net/aspose.cells.drawing/shape/alternativetext/
---
## Shape.AlternativeText property

تُرجع أو تُعيّن سلسلة النص الوصفي (البديلة) لكائن [`Shape`](../).

```csharp
public string AlternativeText { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAlternativeTextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // عيّن النص البديل للشكل
            shape.AlternativeText = "A rectangle shape with width 100 and height 200";

            // احفظ المصنف
            workbook.Save("ShapeAlternativeTextDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


