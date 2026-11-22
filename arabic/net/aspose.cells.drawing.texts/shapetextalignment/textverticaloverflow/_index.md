---
title: "ShapeTextAlignment.TextVerticalOverflow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapeTextAlignment. تحصل وتضبط نوع تجاوز النص العمودي لصندوق النص"
type: docs
url: /ar/net/aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow/
---
## ShapeTextAlignment.TextVerticalOverflow property

يحصل على ويضبط نوع تجاوز النص العمودي لمربع النص.

```csharp
public TextOverflowType TextVerticalOverflow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTextVerticalOverflowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);

            // تعيين نص قد يتجاوز عموديًا
            shape.Text = "This is a long text that might overflow vertically if not clipped properly";

            // الحصول على محاذاة النص وتعيين تجاوز العمودي إلى Clip
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;

            // احفظ المصنف
            workbook.Save("TextVerticalOverflowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextOverflowType](../../../aspose.cells.drawing/textoverflowtype/)
* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


