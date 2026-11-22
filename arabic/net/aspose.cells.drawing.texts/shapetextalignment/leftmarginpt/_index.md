---
title: "ShapeTextAlignment.LeftMarginPt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ShapeTextAlignment. تُرجع الهامش الأيسر بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing.texts/shapetextalignment/leftmarginpt/
---
## ShapeTextAlignment.LeftMarginPt property

يعيد الهامش الأيسر بوحدة النقاط

```csharp
public double LeftMarginPt { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyLeftMarginPtDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلاً مع جميع المعلمات المطلوبة
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            
            // تعيين النص للشكل
            shape.Text = "Sample text with left margin";

            // الوصول إلى محاذاة النص وتعيين الهامش الأيسر بالنقاط
            ShapeTextAlignment textAlignment = shape.TextBody.TextAlignment;
            textAlignment.LeftMarginPt = 2.0d;

            // احفظ المصنف
            workbook.Save("ShapeTextAlignmentLeftMarginPtDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


