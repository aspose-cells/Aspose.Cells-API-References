---
title: "PatternFill.BackTransparency"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PatternFill. تحصل أو تعين شفافية لون الخلفية"
type: docs
url: /ar/net/aspose.cells.drawing/patternfill/backtransparency/
---
## PatternFill.BackTransparency property

الحصول على أو تعيين شفافية لون الخلفية.

```csharp
public double BackTransparency { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyBackTransparencyDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً مستطيلًا إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);

            // الحصول على نسخة PatternFill الموجودة من الشكل وتكوين الخصائص
            shape.Fill.FillType = FillType.Pattern;
            PatternFill patternFill = shape.Fill.PatternFill;
            patternFill.Pattern = FillPattern.Solid;
            patternFill.BackgroundColor = Color.Blue;

            // عرض قيمة BackTransparency الأولية
            Console.WriteLine("Current BackTransparency value: " + patternFill.BackTransparency);

            // تعيين قيمة BackTransparency جديدة (شفافية 50٪)
            patternFill.BackTransparency = 0.5;

            // احفظ المصنف المعدل
            workbook.Save("PatternFillBackTransparencyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


