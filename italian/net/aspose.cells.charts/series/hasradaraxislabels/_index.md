---
title: "Series.HasRadarAxisLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. True se un grafico radar ha etichette dell'asse di categoria. Si applica solo ai grafici radar"
type: docs
url: /it/net/aspose.cells.charts/series/hasradaraxislabels/
---
## Series.HasRadarAxisLabels property

Vero se un grafico radar ha etichette dell'asse di categoria. Si applica solo ai grafici radar.

```csharp
public bool HasRadarAxisLabels { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico radar
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(2);
            worksheet.Cells["B4"].PutValue(5);

            // Aggiungi un grafico radar
            int chartIndex = worksheet.Charts.Add(ChartType.Radar, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi dati della serie
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni la serie e imposta le etichette dell'asse radar
            Series series = chart.NSeries[seriesIndex];
            series.HasRadarAxisLabels = true; // This is the key property being demonstrated

            // Salva la cartella di lavoro
            workbook.Save("RadarChartWithAxisLabels.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


