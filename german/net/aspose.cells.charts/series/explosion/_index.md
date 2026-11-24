---
title: "Series.Explosion"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Series‑Eigenschaft. Der Abstand eines offenen Kuchensegments vom Mittelpunkt des Kuchendiagramms wird als Prozentsatz des Durchmessers des Kuchens angegeben."
type: docs
url: /de/net/aspose.cells.charts/series/explosion/
---
## Series.Explosion property

Der Abstand eines offenen Kuchenstücks vom Mittelpunkt des Kreisdiagramms wird als Prozentsatz des Durchmessers des Kreises angegeben.

```csharp
public int Explosion { get; set; }
```

### Beispiele

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
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Kuchendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Serie hinzufügen
            int seriesIndex = chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";
            
            // Greife auf die Serie zu und setze die Explosion
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
            series.Explosion = 15; // Set explosion value (0-100)
            
            workbook.Save("PieChartExplosionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


