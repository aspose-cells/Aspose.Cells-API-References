---
title: "ChartArea.HeightRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartArea. Ottiene o imposta lo spostamento verticale dalla riga dell'angolo inferiore destro in unità di rapporto dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartarea/heightratiotochart/
---
## ChartArea.HeightRatioToChart property

Restituisce o imposta lo spostamento verticale dalla riga dell'angolo inferiore destro, in unità di rapporto dell'area del grafico.

```csharp
public override double HeightRatioToChart { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyHeightRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Accedi all'area del grafico
            ChartArea chartArea = chart.ChartArea;

            // Visualizza il valore corrente di HeightRatioToChart
            Console.WriteLine("Current HeightRatioToChart value: " + chartArea.HeightRatioToChart);

            // Imposta un nuovo valore per HeightRatioToChart (0,5 = 50% dell'altezza del grafico)
            chartArea.HeightRatioToChart = 0.5;
            Console.WriteLine("New HeightRatioToChart value: " + chartArea.HeightRatioToChart);

            // Imposta un nuovo valore per WidthRatioToChart per dimostrare l'effetto combinato
            chartArea.WidthRatioToChart = 0.8;

            // Salva la cartella di lavoro per vedere le modifiche
            workbook.Save("ChartAreaPropertyHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


