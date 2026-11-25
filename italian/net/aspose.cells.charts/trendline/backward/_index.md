---
title: "Trendline.Backward"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Trendline. Restituisce o imposta il numero di periodi o unità su un grafico a dispersione a cui la trendline si estende all'indietro. Il numero di periodi deve essere maggiore o uguale a zero. Se il tipo di grafico è a colonne, il numero di periodi deve essere compreso tra 0 e 0.5"
type: docs
url: /it/net/aspose.cells.charts/trendline/backward/
---
## Trendline.Backward property

Restituisce o imposta il numero di periodi (o unità in un grafico a dispersione) a cui la linea di tendenza si estende all'indietro. Il numero di periodi deve essere maggiore o uguale a zero. Se il tipo di grafico è a colonne, il numero di periodi deve essere compreso tra 0 e 0,5

```csharp
public double Backward { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyBackwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Crea grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // Aggiungi una trendline e ottienila per indice
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(Aspose.Cells.Charts.TrendlineType.Linear);
            Aspose.Cells.Charts.Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            trendline.DisplayEquation = true;
            
            // Imposta la proprietà backward per estendere la trendline all'indietro di 0.5 unità
            trendline.Backward = 0.5;
            
            workbook.Save("TrendlineBackwardDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


