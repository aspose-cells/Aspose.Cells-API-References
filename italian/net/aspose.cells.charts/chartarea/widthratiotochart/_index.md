---
title: "ChartArea.WidthRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartArea. Ottiene o imposta lo spostamento orizzontale dalla colonna dell'angolo inferiore destro in unità di rapporto dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartarea/widthratiotochart/
---
## ChartArea.WidthRatioToChart property

Restituisce o imposta lo spostamento orizzontale dalla colonna dell'angolo inferiore destro, in unità di rapporto dell'area del grafico.

```csharp
public override double WidthRatioToChart { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyWidthRatioToChartDemo
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

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico
            chart.Calculate();

            // Dimostra la proprietà WidthRatioToChart
            Console.WriteLine("Chart Area Width Ratio: " + chart.ChartArea.WidthRatioToChart);
            
            // Modifica il rapporto e mostra il cambiamento
            chart.ChartArea.WidthRatioToChart = 0.8;
            Console.WriteLine("Modified Chart Area Width Ratio: " + chart.ChartArea.WidthRatioToChart);
        }
    }
}
```

### Vedi anche

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


