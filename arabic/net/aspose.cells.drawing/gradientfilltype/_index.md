---
title: "تعداد GradientFillType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.GradientFillType enum. يمثل جميع أنواع تعبئة التدرج"
type: docs
url: /ar/net/aspose.cells.drawing/gradientfilltype/
---
## GradientFillType enumeration

يمثل جميع أنواع تعبئة التدرج.

```csharp
public enum GradientFillType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Linear | `0` | خطّي |
| Radial | `1` | قطري |
| Rectangle | `2` | مستطيل |
| Path | `3` | مسار |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassGradientFillTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل لتوضيح تعبئة التدرج
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 20);

            // احصل على تنسيق التعبئة
            FillFormat fillFormat = shape.Fill;

            // تعيين نوع تعبئة التدرج والخصائص
            fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.Horizontal, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // إخراج نوع اتجاه التدرج
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // احفظ المصنف
            workbook.Save("GradientFillTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


