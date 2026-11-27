---
title: "Trendline.DataLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Trendline-egenskap. Representerar DataLabels-objektet för den angivna serien"
type: docs
url: /sv/net/aspose.cells.charts/trendline/datalabels/
---
## Trendline.DataLabels property

Representerar DataLabels-objektet för den angivna serien.

```csharp
public DataLabels DataLabels { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDataLabelsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // Skapa diagram
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Lägg till serie och ange trendlinje
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries[0].XValues = "A2:A10";
            chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "Linear Trend");

            // Konfigurera DataLabels för trendlinje
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            trendline.DataLabels.ShowValue = true;
            trendline.DataLabels.Font.Color = Color.Red;
            trendline.DataLabels.Font.IsBold = true;
            trendline.DataLabels.Position = LabelPositionType.Above;
            trendline.DataLabels.Border.IsVisible = true;
            trendline.DataLabels.Border.Color = Color.Black;

            // Spara arbetsboken
            workbook.Save("TrendlineDataLabelsDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataLabels](../../datalabels/)
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


