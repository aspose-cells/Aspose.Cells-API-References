---
title: "Title.YRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Title. Ottiene o imposta la coordinata y dell'angolo in alto a sinistra in unità di frazione dell'area del grafico. Y in pixel  YRatioToChart  Chart.ChartObject.Width"
type: docs
url: /it/net/aspose.cells.charts/title/yratiotochart/
---
## Title.YRatioToChart property

Ottiene o imposta la coordinata y dell'angolo in alto a sinistra in unità di frazione dell'area del grafico. Y in pixel = YRatioToChart * Chart.ChartObject.Width;

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

    public class TitlePropertyYRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni il titolo del grafico
            chart.Title.Text = "Sample Chart Title";
            Title chartTitle = chart.Title;

            // Visualizza il valore corrente di YRatioToChart
            Console.WriteLine("Current YRatioToChart value: " + chartTitle.YRatioToChart);

            // Modifica la proprietà YRatioToChart per spostare il titolo verticalmente
            chartTitle.YRatioToChart = 0.1; // 10% from the top of the chart area
            Console.WriteLine("New YRatioToChart value: " + chartTitle.YRatioToChart);

            // Salva la cartella di lavoro
            workbook.Save("TitlePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


