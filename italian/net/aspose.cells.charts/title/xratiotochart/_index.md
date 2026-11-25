---
title: "Title.XRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Title. Ottiene o imposta la coordinata x dell'angolo in alto a sinistra in unità di frazione dell'area del grafico. X in pixel  XRatioToChart  Chart.ChartObject.Width"
type: docs
url: /it/net/aspose.cells.charts/title/xratiotochart/
---
## Title.XRatioToChart property

Ottiene o imposta la coordinata x dell'angolo in alto a sinistra in unità di frazione dell'area del grafico. X in pixel = XRatioToChart * Chart.ChartObject.Width;

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

    public class TitlePropertyXRatioToChartDemo
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

            // Imposta l'origine dati per il grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni il titolo del grafico
            chart.Title.Text = "Sample Chart Title";
            Title title = chart.Title;

            // Visualizza il valore corrente di XRatioToChart
            Console.WriteLine("Current XRatioToChart value: " + title.XRatioToChart);

            // Modifica il valore di XRatioToChart per spostare il titolo orizzontalmente
            title.XRatioToChart = 0.25; // 25% from the left of the chart area
            Console.WriteLine("New XRatioToChart value: " + title.XRatioToChart);

            // Salva la cartella di lavoro
            workbook.Save("TitlePropertyXRatioToChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


