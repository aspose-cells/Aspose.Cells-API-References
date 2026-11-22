---
title: "ShapeTextAlignment.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeTextAlignment. تحدد ما إذا كانت هذه الحالة لها نفس القيمة ككائن ShapeTextAlignment آخر محدد"
type: docs
url: /ar/net/aspose.cells.drawing.texts/shapetextalignment/equals/
---
## ShapeTextAlignment.Equals method

تحدد ما إذا كانت هذه الحالة لها نفس القيمة ككائن [`ShapeTextAlignment`](../) محدد.

```csharp
public override bool Equals(object obj)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | Object | كائن [`ShapeTextAlignment`](../) للمقارنة مع هذه الحالة. |

### قيمة الإرجاع

صحيح إذا كانت قيمة المعامل obj هي نفسها قيمة هذه المثيلة؛ وإلا، خطأ. إذا كان obj فارغًا، تُعيد هذه الطريقة خطأ.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف شكلاً لمقارنة محاذاة النص
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            
            // احصل على محاذاة نص شكل آخر للمقارنة
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 1, 0, 100, 100);
            ShapeTextAlignment obj = shape2.TextBody.TextAlignment;

            if (shapeTextAlignment.Equals((object)obj))
            {
                Console.WriteLine("Text alignments are equal");
            }
            else
            {
                Console.WriteLine("Text alignments are not equal");
            }
        }
    }
}
```

### انظر أيضًا

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


