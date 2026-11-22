---
title: "ShapeTextAlignment.IsTextWrapped"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapeTextAlignment. تحصل أو تضبط نوع تغليف النص للشكل الذي يحتوي على نص"
type: docs
url: /ar/net/aspose.cells.drawing.texts/shapetextalignment/istextwrapped/
---
## ShapeTextAlignment.IsTextWrapped property

يحصل على أو يضبط نوع التفاف النص للشكل الذي يحتوي على نص.

```csharp
public bool IsTextWrapped { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // تعيين نص الشكل
            shape.Text = "This is a long text that should be wrapped when IsTextWrapped is set to true";

            // الحصول على محاذاة النص وتعيين IsTextWrapped
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            shapeTextAlignment.IsTextWrapped = true;

            // احفظ المصنف
            workbook.Save("ShapeTextWrappingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


