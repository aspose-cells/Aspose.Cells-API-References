---
title: "GradientFill.DirectionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GradientFill. الحصول على نوع اتجاه التدرج"
type: docs
url: /ar/net/aspose.cells.drawing/gradientfill/directiontype/
---
## GradientFill.DirectionType property

يحصل على نوع اتجاه التدرج.

```csharp
public GradientDirectionType DirectionType { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyDirectionTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل لتوضيح تعبئة التدرج
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 5);

            // تعيين خصائص تعبئة التدرج
            FillFormat fillFormat = shape.Fill;
            fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.DiagonalDown, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // إخراج نوع اتجاه التدرج
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // احفظ المصنف
            workbook.Save("GradientDirectionTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


