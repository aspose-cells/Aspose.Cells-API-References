---
title: "التعداد GradientColorType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.GradientColorType enum. يمثل نوع لون التدرج للتعبئة المحددة"
type: docs
url: /ar/net/aspose.cells.drawing/gradientcolortype/
---
## GradientColorType enumeration

يمثل نوع لون التدرج للتعبئة المحددة.

```csharp
public enum GradientColorType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | بدون لون تدرج |
| OneColor | `1` | لون تدرج واحد |
| PresetColors | `2` | ألوان تدرج محددة مسبقًا |
| TwoColors | `3` | لونين متدرجين |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGradientColorTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أضف شكلاً لتوضيح تعبئة التدرج
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
                FillFormat fill = shape.Fill;

                // تعيين نوع تعبئة التدرج
                fill.FillType = FillType.Gradient;

                // عرض قيم تعداد GradientColorType المختلفة
                Console.WriteLine("Available GradientColorType values:");
                Console.WriteLine("None: " + GradientColorType.None);
                Console.WriteLine("OneColor: " + GradientColorType.OneColor);
                Console.WriteLine("PresetColors: " + GradientColorType.PresetColors);
                Console.WriteLine("TwoColors: " + GradientColorType.TwoColors);

                // قراءة وعرض نوع لون التدرج الحالي (الخاصية للقراءة فقط)
                Console.WriteLine("Current gradient color type: " + fill.GradientColorType);

                // احفظ المصنف
                workbook.Save("GradientColorTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientColorType: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


