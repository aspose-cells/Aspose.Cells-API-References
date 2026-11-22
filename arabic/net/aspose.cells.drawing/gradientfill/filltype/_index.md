---
title: "GradientFill.FillType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GradientFill. يحصل على نوع تعبئة التدرج"
type: docs
url: /ar/net/aspose.cells.drawing/gradientfill/filltype/
---
## GradientFill.FillType property

يحصل على نوع تعبئة التدرج.

```csharp
public GradientFillType FillType { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyFillTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل مع تعبئة تدرج
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            FillFormat fillFormat = shape.Fill;
            fillFormat.FillType = FillType.Gradient;
            
            // تعيين خصائص التدرج
            GradientFill gradientFill = fillFormat.GradientFill;
            gradientFill.SetTwoColorGradient(System.Drawing.Color.Red, System.Drawing.Color.Blue, GradientStyleType.Horizontal, 1);
            
            // عرض نوع تعبئة التدرج
            Console.WriteLine("Gradient Fill Type: " + gradientFill.FillType);
            
            // تغيير إلى تدرج شعاعي
            gradientFill.SetGradient(GradientFillType.Radial, 45, GradientDirectionType.FromCenter);
            Console.WriteLine("Updated Gradient Fill Type: " + gradientFill.FillType);
            
            // احفظ المصنف
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [GradientFillType](../../gradientfilltype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


