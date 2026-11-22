---
title: "Axis.IsAutomaticMinValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تشير إلى ما إذا كانت القيمة الدنيا تُعيّن تلقائيًا"
type: docs
url: /ar/net/aspose.cells.charts/axis/isautomaticminvalue/
---
## Axis.IsAutomaticMinValue property

يشير إلى ما إذا كانت القيمة الدنيا تُعيّن تلقائيًا.

```csharp
public bool IsAutomaticMinValue { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutomaticMinValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // قم بتكوين محور القيم
            Axis valueAxis = chart.ValueAxis;
            valueAxis.IsAutomaticMinValue = false;
            valueAxis.MinValue = 0;
            valueAxis.IsAutomaticMaxValue = true; // Keep max value automatic for contrast
            
            // حفظ النتيجة
            workbook.Save("AxisPropertyIsAutomaticMinValueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


