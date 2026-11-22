---
title: "Trendline.DisplayRSquared"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Trendline. تمثّل ما إذا كانت قيمة Rsquared لخط الاتجاه تُعرض على المخطط في نفس تسمية البيانات مع المعادلة. تعيين هذه الخاصية إلى True يُفعّل تلقائيًا تسميات البيانات"
type: docs
url: /ar/net/aspose.cells.charts/trendline/displayrsquared/
---
## Trendline.DisplayRSquared property

يمثل ما إذا كانت قيمة R-squared لخط الاتجاه معروضة على المخطط (في نفس تسمية البيانات كالمعادلة). ضبط هذه الخاصية على True يُفعِّل تلقائيًا تسميات البيانات.

```csharp
public bool DisplayRSquared { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDisplayRSquaredDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(4);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(6);
            worksheet.Cells["B4"].PutValue(8);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // أضف خط اتجاه واحصل عليه حسب الفهرس
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            
            // عرض خاصية DisplayRSquared
            trendline.DisplayRSquared = true;
            trendline.DisplayEquation = true;

            // احفظ المصنف
            workbook.Save("TrendlineDisplayRSquaredDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


