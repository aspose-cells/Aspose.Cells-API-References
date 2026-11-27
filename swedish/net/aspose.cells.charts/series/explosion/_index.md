---
title: "Series.Explosion"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series‑egenskap. Avståndet för en öppen pajskiva från mitten av pajdiagrammet uttrycks som en procentsats av pajens diameter"
type: docs
url: /sv/net/aspose.cells.charts/series/explosion/
---
## Series.Explosion property

Avståndet för ett öppet pajsegment från centrum av pajdiagrammet uttrycks som en procentandel av pajens diameter.

```csharp
public int Explosion { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyExplosionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Lägg till pajdiagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serie
            int seriesIndex = chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";
            
            // Åtkomst till serien och ange explosion
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
            series.Explosion = 15; // Set explosion value (0-100)
            
            workbook.Save("PieChartExplosionDemo.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


