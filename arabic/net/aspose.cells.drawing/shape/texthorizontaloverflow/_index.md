---
title: "Shape.TextHorizontalOverflow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. يحصل ويضبط نوع تجاوز النص الأفقي للشكل الذي يحتوي على نص"
type: docs
url: /ar/net/aspose.cells.drawing/shape/texthorizontaloverflow/
---
## Shape.TextHorizontalOverflow property

يحصل ويضبط نوع تدفق النص الأفقي للشكل الذي يحتوي على نص.

```csharp
public TextOverflowType TextHorizontalOverflow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextHorizontalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل صندوق نص مع المعلمات الصحيحة
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            textBox.Text = "This is a long text that will demonstrate text horizontal overflow functionality";

            // تعيين نوع التجاوز الأولي إلى Clip
            textBox.TextHorizontalOverflow = TextOverflowType.Clip;
            Console.WriteLine("TextHorizontalOverflow set to Clip (text will be clipped)");

            // تغيير نوع التجاوز إلى Overflow
            textBox.TextHorizontalOverflow = TextOverflowType.Overflow;
            Console.WriteLine("TextHorizontalOverflow changed to Overflow (text will overflow)");

            // احفظ المصنف
            workbook.Save("TextHorizontalOverflowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextOverflowType](../../textoverflowtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


