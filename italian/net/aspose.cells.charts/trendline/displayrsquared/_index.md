---
title: "Trendline.DisplayRSquared"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Trendline. Indica se il valore Rsquared della trendline è visualizzato sul grafico nella stessa etichetta dati dell'equazione. Impostare questa proprietà su True attiva automaticamente le etichette dati"
type: docs
url: /it/net/aspose.cells.charts/trendline/displayrsquared/
---
## Trendline.DisplayRSquared property

Indica se il valore R-quadrato della linea di tendenza è visualizzato sul grafico (nella stessa etichetta dati dell'equazione). Impostare questa proprietà su True attiva automaticamente le etichette dati.

```csharp
public bool DisplayRSquared { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDisplayRSquaredDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(4);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(6);
            worksheet.Cells["B4"].PutValue(8);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // Aggiungi una trendline e ottienila per indice
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            
            // Dimostrare la proprietà DisplayRSquared
            trendline.DisplayRSquared = true;
            trendline.DisplayEquation = true;

            // Salva la cartella di lavoro
            workbook.Save("TrendlineDisplayRSquaredDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


