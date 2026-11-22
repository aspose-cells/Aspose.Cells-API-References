---
title: "ShapeTextAlignment.TextHorizontalOverflow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapeTextAlignment. تحصّل وتضبط نوع تدفق النص الأفقي في مربع النص"
type: docs
url: /ar/net/aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow/
---
## ShapeTextAlignment.TextHorizontalOverflow property

يحصل على ويضبط نوع تجاوز النص الأفقي لمربع النص.

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
    public class ShapeTextAlignmentPropertyTextHorizontalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مربع نص
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 50);
            textBox.Text = "This is a long text that demonstrates horizontal overflow behavior";

            // تعيين تدفق أفقي إلى Clip
            textBox.TextBody.TextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;

            // احفظ المصنف
            workbook.Save("TextHorizontalOverflowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextOverflowType](../../../aspose.cells.drawing/textoverflowtype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


