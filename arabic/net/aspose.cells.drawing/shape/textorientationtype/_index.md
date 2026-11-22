---
title: "Shape.TextOrientationType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الشكل. تحصل وتعيّن نوع توجيه النص في الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/textorientationtype/
---
## Shape.TextOrientationType property

يحصل ويضبط نوع توجيه النص للشكل.

```csharp
public TextOrientationType TextOrientationType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextOrientationTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // تعيين النص للشكل
            shape.Text = "Sample Text";

            // التحقق من توجيه النص وتعديله
            if (shape.TextOrientationType == TextOrientationType.NoRotation)
            {
                shape.TextOrientationType = TextOrientationType.TopToBottom;
            }

            // احفظ المصنف
            workbook.Save("ShapeTextOrientationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextOrientationType](../../../aspose.cells/textorientationtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


