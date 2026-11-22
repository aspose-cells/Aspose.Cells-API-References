---
title: "GradientFill.Angle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GradientFill. زاوية التعبئة الخطية"
type: docs
url: /ar/net/aspose.cells.drawing/gradientfill/angle/
---
## GradientFill.Angle property

زاوية التعبئة الخطية.

```csharp
public float Angle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyAngleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً لتوضيح تعبئة التدرج
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // تعيين خصائص تعبئة التدرج
            shape.Fill.FillType = FillType.Gradient;
            shape.Fill.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromCenter);
            shape.Fill.GradientFill.Angle = 45; // Set the angle to 45 degrees

            // تعيين ألوان التدرج
            shape.Fill.GradientFill.SetTwoColorGradient(
                Color.Red, 
                Color.Blue, 
                GradientStyleType.Horizontal, 
                1);

            // احفظ المصنف
            workbook.Save("GradientFillAngleDemo.xlsx");

            Console.WriteLine("Demo completed. File saved with gradient fill at 45 degree angle.");
        }
    }
}
```

### انظر أيضًا

* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


