---
title: "FillFormat.PresetColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FillFormat. تُرجع لون التدرج المحدد للملء المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/fillformat/presetcolor/
---
## FillFormat.PresetColor property

يعيد لون التدرج المسبق للملء المحدد.

```csharp
public GradientPresetType PresetColor { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPresetColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // الوصول إلى تنسيق الملء لمنطقة المخطط
            FillFormat fillFormat = chart.ChartArea.Area.FillFormat;

            // تعيين لون تدرج محدد
            fillFormat.SetPresetColorGradient(GradientPresetType.Ocean, GradientStyleType.DiagonalUp, 2);

            // عرض والتحقق من اللون المحدد
            Console.WriteLine("Preset Color: " + fillFormat.PresetColor);

            // احفظ المصنف
            workbook.Save("FillFormatPresetColorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [GradientPresetType](../../gradientpresettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


