---
title: "Chart.ChartArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Chart. تحصل على مساحة المخطط في ورقة العمل"
type: docs
url: /ar/net/aspose.cells.charts/chart/chartarea/
---
## Chart.ChartArea property

يحصل على مساحة المخطط في ورقة العمل.

```csharp
public ChartArea ChartArea { get; }
```

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyChartAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(70);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            ChartArea chartArea = chart.ChartArea;
            chartArea.Border.Weight = WeightType.SingleLine;
            chartArea.Border.Color = System.Drawing.Color.Blue;

            workbook.Save("ChartPropertyChartAreaDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartArea](../../chartarea/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


