---
title: "ChartFrame.HeightRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Ottiene o imposta l'altezza del frame in unità del rapporto dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartframe/heightratiotochart/
---
## ChartFrame.HeightRatioToChart property

Ottiene o imposta l'altezza del frame in unità del rapporto dell'area del grafico.

```csharp
public virtual double HeightRatioToChart { get; set; }
```

### Osservazioni

Questo è un valore frazionario, il suo intervallo valido è tra 0-1. Come convertire le unità di rapporto in pixel? HeightPixel = HeightRatioToChart * Chart.ChartObject.Height;

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightRatioToChartDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi al titolo del grafico (che eredita da ChartFrame)
            chart.Title.Text = "Sample Chart";
            ChartFrame titleFrame = chart.Title;

            // Visualizza il valore corrente di HeightRatioToChart
            Console.WriteLine("Current HeightRatioToChart value: " + titleFrame.HeightRatioToChart);

            // Imposta un nuovo rapporto di altezza (0.1 = 10% dell'altezza del grafico)
            titleFrame.HeightRatioToChart = 0.1;

            // Dimostra l'effetto confrontando prima/dopo
            Console.WriteLine("Title height reduced to 10% of chart height");

            // Salva il risultato
            workbook.Save("PropertyHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


