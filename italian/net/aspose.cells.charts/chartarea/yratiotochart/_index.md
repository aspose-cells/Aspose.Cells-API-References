---
title: "ChartArea.YRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartArea. Ottiene o imposta lo spostamento verticale dalla riga dell'angolo superiore sinistro in unità di rapporto dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartarea/yratiotochart/
---
## ChartArea.YRatioToChart property

Restituisce o ottiene lo spostamento verticale dalla riga dell'angolo superiore sinistro, in unità di rapporto dell'area del grafico.

```csharp
public override double YRatioToChart { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyYRatioToChartDemo
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
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi all'area del grafico
            ChartArea chartArea = chart.ChartArea;

            // Visualizza il valore corrente di YRatioToChart
            Console.WriteLine("Current YRatioToChart value: " + chartArea.YRatioToChart);

            // Modifica la proprietà YRatioToChart (0,0 a 1,0 rappresentano lo 0% al 100% dell'area del grafico)
            chartArea.YRatioToChart = 0.2; // Move chart area down by 20% of chart height

            // Visualizza il nuovo valore di YRatioToChart
            Console.WriteLine("New YRatioToChart value: " + chartArea.YRatioToChart);

            // Salva la cartella di lavoro per vedere l'effetto
            workbook.Save("ChartAreaPropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


