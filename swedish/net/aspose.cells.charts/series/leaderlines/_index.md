---
title: "Series.LeaderLines"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Representerar ledarlinjer i ett diagram. Ledarlinjer kopplar datamärkningar till datapunkter. Detta objekt är inte en samling; det finns inget objekt som representerar en enskild ledarlinje"
type: docs
url: /sv/net/aspose.cells.charts/series/leaderlines/
---
## Series.LeaderLines property

Representerar ledarlinjer i ett diagram. Ledarlinjer kopplar datamärkningar till datapunkter. Detta objekt är inte en samling; det finns inget objekt som representerar en enskild ledarlinje.

```csharp
public Line LeaderLines { get; }
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
    public class SeriesPropertyLeaderLinesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett pajdiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Konfigurera datamärkningar
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShowPercentage = true;
            series.DataLabels.Position = LabelPositionType.OutsideEnd;

            // Konfigurera ledarlinjer
            series.HasLeaderLines = true;
            series.LeaderLines.IsAuto = false;
            series.LeaderLines.Style = LineType.Dot;
            series.LeaderLines.WeightPt = 1.5;
            series.LeaderLines.Color = Color.Blue;

            // Spara arbetsboken
            workbook.Save("SeriesPropertyLeaderLinesDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


