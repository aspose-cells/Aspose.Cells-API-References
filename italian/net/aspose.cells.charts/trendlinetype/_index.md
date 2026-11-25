---
title: "Enum TrendlineType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Charts.TrendlineType. Rappresenta il tipo di linea di tendenza"
type: docs
url: /it/net/aspose.cells.charts/trendlinetype/
---
## TrendlineType enumeration

Rappresenta il tipo di linea di tendenza.

```csharp
public enum TrendlineType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Exponential | `0` | Esponenziale |
| Linear | `1` | Lineare |
| Logarithmic | `2` | Logaritmico |
| MovingAverage | `3` | MediaMobile |
| Polynomial | `4` | Polinomiale |
| Power | `5` | Potenza |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class TrendlineTypeDemo
    {
        public static void TrendlineTypeExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            
            // Aggiunta di un nuovo foglio di lavoro all'oggetto Excel
            int sheetIndex = workbook.Worksheets.Add();
            
            // Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Aggiunta di valori di esempio alle celle
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Aggiunta di un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Accesso all'istanza del grafico appena aggiunto
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiunta di NSeries (origine dati del grafico) al grafico che va dalla cella "A1" alla "B4"
            chart.NSeries.Add("A1:B4", true);
            
            // Impostazione dell'origine dati per i dati di categoria di NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Aggiunta di diversi tipi di linee di tendenza al grafico
            AddTrendline(chart, 0, TrendlineType.Linear, "Linear Trendline");
            AddTrendline(chart, 0, TrendlineType.Exponential, "Exponential Trendline");
            AddTrendline(chart, 0, TrendlineType.Logarithmic, "Logarithmic Trendline");
            AddTrendline(chart, 0, TrendlineType.MovingAverage, "Moving Average Trendline");
            AddTrendline(chart, 0, TrendlineType.Polynomial, "Polynomial Trendline");
            AddTrendline(chart, 0, TrendlineType.Power, "Power Trendline");

            // Salvataggio del file Excel
            workbook.Save("TrendlineTypeExample.xlsx");
        }

        private static void AddTrendline(Chart chart, int seriesIndex, TrendlineType trendlineType, string trendlineName)
        {
            // Aggiunta di una linea di tendenza del tipo specificato alla serie specificata
            int index = chart.NSeries[seriesIndex].TrendLines.Add(trendlineType);
            Trendline trendline = chart.NSeries[seriesIndex].TrendLines[index];
            
            // Impostazione del nome personalizzato della linea di tendenza
            trendline.Name = trendlineName;
            
            // Visualizzazione dell'equazione sul grafico
            trendline.DisplayEquation = true;
            
            // Visualizzazione del valore R-quadrato sul grafico
            trendline.DisplayRSquared = true;
            
            // Impostazione del colore della linea di tendenza
            trendline.Color = Color.Red;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


