---
title: "ShapeTextAlignment.RightMarginPt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapeTextAlignment. تُعيد الهامش الأيمن بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing.texts/shapetextalignment/rightmarginpt/
---
## ShapeTextAlignment.RightMarginPt property

يعيد الهامش الأيمن بوحدة النقاط

```csharp
public double RightMarginPt { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyRightMarginPtDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // الوصول إلى محاذاة النص
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // حدد الهامش الأيمن بالنقاط
            shapeTextAlignment.RightMarginPt = 2.0d;

            // تحقق من الخاصية عن طريق استرجاع القيمة
            Console.WriteLine("Right Margin in Points: " + shapeTextAlignment.RightMarginPt);
        }
    }
}
```

### انظر أيضًا

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


