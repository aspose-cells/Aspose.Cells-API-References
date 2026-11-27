---
title: "ChartPoint.XValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartPoint-egenskap. Hämtar eller sätter X‑värdet för diagrampunkten"
type: docs
url: /sv/net/aspose.cells.charts/chartpoint/xvalue/
---
## ChartPoint.XValue property

Hämtar eller anger X‑värdet för diagrampunkten.

```csharp
public object XValue { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyXValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägger till exempeldata
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(50);
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);

            // Lägger till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställer in diagrammets datakälla
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Anpassar datapunkterna
            for (int i = 0; i < chart.NSeries[0].Points.Count; i++)
            {
                ChartPoint point = chart.NSeries[0].Points[i];
                
                // Demonstrerar användning av XValue‑egenskapen
                point.XValue = "Modified " + (i + 1);
                
                // Ytterligare formatering för synlighet
                point.Area.ForegroundColor = Color.FromArgb(100 + i * 50, 150, 200);
            }

            workbook.Save("ChartPointXValueDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


