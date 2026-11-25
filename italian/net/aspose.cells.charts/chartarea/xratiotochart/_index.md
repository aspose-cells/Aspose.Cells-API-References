---
title: "ChartArea.XRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartArea. Ottiene o imposta lo spostamento orizzontale dalla colonna dell'angolo superiore sinistro come rapporto dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartarea/xratiotochart/
---
## ChartArea.XRatioToChart property

Restituisce o imposta lo spostamento orizzontale dalla colonna dell'angolo superiore‑sinistro, come rapporto dell'area del grafico.

```csharp
public override double XRatioToChart { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyXRatioToChartDemo
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

            // Ottieni l'area del grafico
            ChartArea chartArea = chart.ChartArea;

            // Visualizza il valore corrente di XRatioToChart
            Console.WriteLine("Current XRatioToChart value: " + chartArea.XRatioToChart);

            // Cambia il valore di XRatioToChart per spostare l'area del grafico orizzontalmente
            chartArea.XRatioToChart = 0.2; // 20% from the left of the chart container

            // Visualizza il nuovo valore di XRatioToChart
            Console.WriteLine("New XRatioToChart value: " + chartArea.XRatioToChart);

            // Salva la cartella di lavoro
            workbook.Save("ChartAreaXRatioToChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


