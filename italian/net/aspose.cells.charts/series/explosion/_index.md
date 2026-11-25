---
title: "Series.Explosion"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà della serie. La distanza di una fetta di torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta"
type: docs
url: /it/net/aspose.cells.charts/series/explosion/
---
## Series.Explosion property

La distanza di una fetta di torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta.

```csharp
public int Explosion { get; set; }
```

### Esempi

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
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Aggiungi grafico a torta
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie
            int seriesIndex = chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";
            
            // Accedi alla serie e imposta l'explosion
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
            series.Explosion = 15; // Set explosion value (0-100)
            
            workbook.Save("PieChartExplosionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


