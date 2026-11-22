---
title: "Trendline.DisplayEquation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Trendline. تمثل ما إذا كانت معادلة خط الاتجاه معروضة على المخطط في نفس تسمية البيانات كقيمة R المربعة. ضبط هذه الخاصية على True يُفعّل تلقائيًا تسميات البيانات"
type: docs
url: /ar/net/aspose.cells.charts/trendline/displayequation/
---
## Trendline.DisplayEquation property

يمثل ما إذا كانت معادلة خط الاتجاه معروضة على المخطط (في نفس تسمية البيانات كقيمة R-squared). ضبط هذه الخاصية على True يُفعِّل تلقائيًا تسميات البيانات.

```csharp
public bool DisplayEquation { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDisplayEquationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // إنشاء مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة وخط اتجاه
            chart.NSeries.Add("A1:B4", true);
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // تكوين خصائص خط الاتجاه
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = false;
            trendline.Color = Color.Blue;

            workbook.Save("TrendlineDisplayEquationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


