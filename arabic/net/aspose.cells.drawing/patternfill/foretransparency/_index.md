---
title: "PatternFill.ForeTransparency"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PatternFill. تحصل أو تعين شفافية لون المقدمة"
type: docs
url: /ar/net/aspose.cells.drawing/patternfill/foretransparency/
---
## PatternFill.ForeTransparency property

الحصول على أو تعيين شفافية لون الأمام.

```csharp
public double ForeTransparency { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForeTransparencyDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل مستطيل لتوضيح تعبئة النمط
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // عيّن نوع التعبئة إلى نمط
            shape.Fill.FillType = FillType.Pattern;

            // احصل على نسخة PatternFill
            PatternFill patternFill = shape.Fill.PatternFill;

            // تكوين خصائص تعبئة النمط
            patternFill.Pattern = FillPattern.Solid;
            patternFill.ForegroundColor = Color.Red;
            patternFill.BackgroundColor = Color.Blue;

            try
            {
                // عرض قيمة ForeTransparency الأولية
                Console.WriteLine("Initial ForeTransparency value: " + patternFill.ForeTransparency);

                // تعيين قيمة ForeTransparency جديدة (شفافية 50٪)
                patternFill.ForeTransparency = 0.5;

                // عرض قيمة ForeTransparency المحدثة
                Console.WriteLine("Updated ForeTransparency value: " + patternFill.ForeTransparency);

                // احفظ المصنف
                workbook.Save("ForeTransparencyDemo.xlsx");
                Console.WriteLine("ForeTransparency demonstration completed successfully.");
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

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


