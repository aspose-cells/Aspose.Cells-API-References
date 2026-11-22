---
title: "Shape.TextVerticalAlignment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل وتضبط نوع محاذاة النص العمودية للشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/textverticalalignment/
---
## Shape.TextVerticalAlignment property

يحصل ويضبط نوع محاذاة النص العمودية للشكل.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextVerticalAlignmentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // قم بتعيين النص والمحاذاة
            shape.Text = "Vertical Alignment Demo";
            shape.TextVerticalAlignment = TextAlignmentType.Bottom;
            
            Console.WriteLine("Initial Vertical Alignment: " + shape.TextVerticalAlignment);

            // غيّر المحاذاة العمودية
            if (shape.TextVerticalAlignment == TextAlignmentType.Bottom)
            {
                shape.TextVerticalAlignment = TextAlignmentType.Center;
            }

            Console.WriteLine("Updated Vertical Alignment: " + shape.TextVerticalAlignment);

            // احفظ المصنف
            workbook.Save("TextVerticalAlignmentDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


