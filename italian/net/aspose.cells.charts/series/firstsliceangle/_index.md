---
title: "Series.FirstSliceAngle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Ottiene o imposta l'angolo della prima fetta di un piechart o doughnutchart in gradi in senso orario dalla verticale. Si applica solo a pie, 3D pie e doughnut chart con valori da 0 a 360"
type: docs
url: /it/net/aspose.cells.charts/series/firstsliceangle/
---
## Series.FirstSliceAngle property

Ottiene o imposta l'angolo della prima fetta di grafico a torta o a ciambella, in gradi (in senso orario dal verticale). Si applica solo a grafici a torta, a torta 3-D e a ciambella, con valori da 0 a 360.

```csharp
public short FirstSliceAngle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyFirstSliceAngleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico a torta
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Aggiungi grafico a torta
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni la prima serie e imposta FirstSliceAngle
            Series series = chart.NSeries[0];
            series.FirstSliceAngle = 45; // Rotate pie chart by 45 degrees

            workbook.Save("PieChartWithFirstSliceAngle.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


