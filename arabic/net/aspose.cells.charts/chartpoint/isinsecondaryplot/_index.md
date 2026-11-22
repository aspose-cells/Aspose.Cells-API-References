---
title: "ChartPoint.IsInSecondaryPlot"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartPoint. يحصل أو يعيّن قيمة تشير ما إذا كانت هذه النقطة البيانات في الفطيرة الثانية أو الشريط في مخطط pie of pie أو bar of pie."
type: docs
url: /ar/net/aspose.cells.charts/chartpoint/isinsecondaryplot/
---
## ChartPoint.IsInSecondaryPlot property

يحصل أو يعيّن قيمة تشير إلى ما إذا كانت هذه النقطة البيانات في الفطيرة أو الشريط الثاني في مخطط فطيرة داخل فطيرة أو شريط داخل فطيرة.

```csharp
public bool IsInSecondaryPlot { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyIsInSecondaryPlotDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // أنشئ مخطط pie يدعم المخططات الثانوية
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // قم بتكوين المخطط الثانوي
            chart.NSeries[0].Points[2].IsInSecondaryPlot = true;
            chart.NSeries[0].Points[3].IsInSecondaryPlot = true;

            // حفظ الناتج
            workbook.Save("PieChartWithSecondaryPlot.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


