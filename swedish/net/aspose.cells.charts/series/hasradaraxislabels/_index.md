---
title: "Series.HasRadarAxisLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Sant om ett radardiagram har kategori‑axelrubriker. Gäller endast radardiagram."
type: docs
url: /sv/net/aspose.cells.charts/series/hasradaraxislabels/
---
## Series.HasRadarAxisLabels property

Sant om ett radardiagram har kategoriska axelrubriker. Gäller endast radardiagram.

```csharp
public bool HasRadarAxisLabels { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasRadarAxisLabelsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för radardiagram
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(2);
            worksheet.Cells["B4"].PutValue(5);

            // Lägg till ett radardiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Radar, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till seriedata
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta serien och ange radaraxelrubriker.
            Series series = chart.NSeries[seriesIndex];
            series.HasRadarAxisLabels = true; // This is the key property being demonstrated

            // Spara arbetsboken
            workbook.Save("RadarChartWithAxisLabels.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


