---
title: "Trendline.Intercept"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Trendline. تُعيد أو تعيّن النقطة التي يقطع فيها خط الاتجاه محور القيم"
type: docs
url: /ar/net/aspose.cells.charts/trendline/intercept/
---
## Trendline.Intercept property

إرجاع أو تعيين النقطة التي يقطع فيها خط الاتجاه محور القيم.

```csharp
public double Intercept { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyInterceptDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(6);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // إضافة خط اتجاه وتعيين نقطة التقاطع
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Intercept = 1.0; // Setting the Y-intercept value
            trendline.DisplayEquation = true;

            workbook.Save("TrendlineInterceptDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


