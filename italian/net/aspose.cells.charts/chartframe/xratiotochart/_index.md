---
title: "ChartFrame.XRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Ottiene o imposta la coordinata x dell'angolo superiore sinistro in unità di rapporto dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartframe/xratiotochart/
---
## ChartFrame.XRatioToChart property

Ottiene o imposta la coordinata x dell'angolo in alto a sinistra in unità del rapporto dell'area del grafico.

```csharp
public virtual double XRatioToChart { get; set; }
```

### Osservazioni

Questo è un valore frazionario, il suo intervallo valido è compreso tra 0 e 1. Come convertire le unità di rapporto in pixel? XPixel = XRatioToChart * Chart.ChartObject.Width;

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyXRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi al titolo del grafico che è un ChartFrame
            ChartFrame chartTitle = chart.Title;

            // Visualizza il valore corrente di XRatioToChart
            Console.WriteLine("Current XRatioToChart value: " + chartTitle.XRatioToChart);

            // Imposta un nuovo valore XRatioToChart (0.5 significa il 50% della larghezza del grafico da sinistra)
            chartTitle.XRatioToChart = 0.5;

            // Visualizza la nuova posizione
            Console.WriteLine("Title position after change - XRatioToChart: " + chartTitle.XRatioToChart);

            // Salva la cartella di lavoro
            workbook.Save("ChartFrameXRatioToChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


