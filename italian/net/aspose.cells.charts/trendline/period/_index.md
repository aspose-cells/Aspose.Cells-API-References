---
title: "Trendline.Period"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Trendline. Restituisce o imposta il periodo per la trendline movingaverage"
type: docs
url: /it/net/aspose.cells.charts/trendline/period/
---
## Trendline.Period property

Restituisce o imposta il periodo per la linea di tendenza della media mobile.

```csharp
public int Period { get; set; }
```

### Osservazioni

Questo valore dovrebbe essere compreso tra 2 e 255. Inoltre deve essere inferiore al numero di punti del grafico nella serie

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyPeriodDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["B1"].PutValue("Y");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i);
                worksheet.Cells["B" + i].PutValue(i * 2);
            }

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi serie
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries.CategoryData = "A2:A10";

            // Aggiungi una trendline a media mobile
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.MovingAverage);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Period = 3; // Set period for moving average
            trendline.Name = "3-Period Moving Average";

            // Salva la cartella di lavoro
            workbook.Save("TrendlinePeriodDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


