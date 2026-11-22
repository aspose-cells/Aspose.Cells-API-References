---
title: "Trendline.Period"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Trendline. تُرجع أو تُعيّن الفترة لخط الاتجاه المتوسط المتحرك"
type: docs
url: /ar/net/aspose.cells.charts/trendline/period/
---
## Trendline.Period property

يعيد أو يضبط الفترة لخط الاتجاه المتوسط المتحرك.

```csharp
public int Period { get; set; }
```

### ملاحظات

يجب أن تكون هذه القيمة بين 2 و 255. ويجب أن تكون أقل من عدد نقاط المخطط في السلسلة

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyPeriodDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة سلسلة
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // أضف خط اتجاه متوسط متحرك
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.MovingAverage);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Period = 3; // Set period for moving average
            trendline.Name = "3-Period Moving Average";

            // احفظ المصنف
            workbook.Save("TrendlinePeriodDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


