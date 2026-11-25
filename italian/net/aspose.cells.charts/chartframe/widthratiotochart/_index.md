---
title: "ChartFrame.WidthRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Ottiene o imposta la larghezza del frame in unità di rapporto dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartframe/widthratiotochart/
---
## ChartFrame.WidthRatioToChart property

Ottiene o imposta la larghezza del frame in unità del rapporto dell'area del grafico.

```csharp
public virtual double WidthRatioToChart { get; set; }
```

### Osservazioni

Questo è un valore frazionario, il suo intervallo valido è tra 0-1. Come convertire le unità di rapporto in pixel? WidthPixel = WidthRatioToChart * Chart.ChartObject.Width;

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyWidthRatioToChartDemo
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

            // Visualizza il rapporto di larghezza corrente
            Console.WriteLine("Current WidthRatioToChart value: " + chartTitle.WidthRatioToChart);

            // Imposta un nuovo rapporto di larghezza (0.5 = 50% della larghezza del grafico)
            chartTitle.WidthRatioToChart = 0.5;

            // Mostra l'effetto salvando la cartella di lavoro
            workbook.Save("ChartFrameWidthRatioDemo.xlsx");

            Console.WriteLine("WidthRatioToChart property demonstrated successfully.");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


