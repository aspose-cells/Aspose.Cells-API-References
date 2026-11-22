---
title: "ShapeTextAlignment.IsAutoMargin"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapeTextAlignment. تشير إلى ما إذا كان هامش إطار النص تلقائيًا"
type: docs
url: /ar/net/aspose.cells.drawing.texts/shapetextalignment/isautomargin/
---
## ShapeTextAlignment.IsAutoMargin property

يشير إلى ما إذا كان هامش إطار النص تلقائيًا.

```csharp
public bool IsAutoMargin { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsAutoMarginDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // الوصول إلى محاذاة النص وتعيين IsAutoMargin
            shape.TextBody.TextAlignment.IsAutoMargin = true;

            // تعيين بعض النص للتوضيح
            shape.Text = "Sample text with auto margins";

            // احفظ المصنف
            workbook.Save("ShapeTextAlignmentIsAutoMarginDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


