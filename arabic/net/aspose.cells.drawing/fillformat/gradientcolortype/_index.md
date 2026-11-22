---
title: "FillFormat.GradientColorType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FillFormat. تُرجع نوع لون التدرج للتعبئة المحددة"
type: docs
url: /ar/net/aspose.cells.drawing/fillformat/gradientcolortype/
---
## FillFormat.GradientColorType property

يرجع نوع لون التدرج للتعبئة المحددة.

```csharp
public GradientColorType GradientColorType { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertyGradientColorTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً لتوضيح تعبئة التدرج
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            try
            {
                // حدد تعبئة تدرج لوني ثنائي
                shape.Fill.SetTwoColorGradient(Color.Red, Color.Blue,
                    GradientStyleType.Horizontal, 2);

                // الوصول إلى FillFormat للحصول على GradientColorType
                FillFormat fillFormat = shape.Fill;

                // اعرض قيمة GradientColorType
                Console.WriteLine("GradientColorType: " + fillFormat.GradientColorType);

                // احفظ المصنف
                workbook.Save("GradientColorTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [GradientColorType](../../gradientcolortype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


