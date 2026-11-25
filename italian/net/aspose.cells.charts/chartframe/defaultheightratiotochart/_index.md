---
title: "ChartFrame.DefaultHeightRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Rappresenta l'altezza della posizione predefinita in unità della frazione dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartframe/defaultheightratiotochart/
---
## ChartFrame.DefaultHeightRatioToChart property

Rappresenta l'altezza della posizione predefinita in unità di frazione dell'area del grafico.

```csharp
public double DefaultHeightRatioToChart { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultHeightRatioToChartDemo
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

            // Accedi al titolo del grafico (che è un ChartFrame)
            ChartFrame chartTitle = chart.Title;

            // Visualizza il valore corrente di DefaultHeightRatioToChart
            Console.WriteLine("Current DefaultHeightRatioToChart value: " + chartTitle.DefaultHeightRatioToChart);

            // Dimostra come questa proprietà influisce sul grafico confrontandola con HeightRatioToChart
            Console.WriteLine("Current HeightRatioToChart value: " + chartTitle.HeightRatioToChart);

            // Modifica il rapporto di altezza per vedere l'effetto
            chartTitle.HeightRatioToChart = 0.1;
            Console.WriteLine("After setting HeightRatioToChart to 0.1: " + chartTitle.HeightRatioToChart);

            // Salva la cartella di lavoro
            workbook.Save("ChartFramePropertyDefaultHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


