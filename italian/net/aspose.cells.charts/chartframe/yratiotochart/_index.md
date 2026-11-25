---
title: "ChartFrame.YRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Ottiene o imposta la coordinata y dell'angolo in alto a sinistra in unità del rapporto dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartframe/yratiotochart/
---
## ChartFrame.YRatioToChart property

Ottiene o imposta la coordinata y dell'angolo in alto a sinistra in unità del rapporto dell'area del grafico.

```csharp
public virtual double YRatioToChart { get; set; }
```

### Osservazioni

Questo è un valore frazionario, il suo intervallo valido è compreso tra 0-1. Come convertire le unità di rapporto in pixel? YPixel = YRatioToChart * Chart.ChartObject.Height;

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyYRatioToChartDemo
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
            
            // Accedi al titolo del grafico che eredita da ChartFrame
            chart.Title.Text = "Sample Chart";
            
            // Visualizza il valore corrente di YRatioToChart
            Console.WriteLine("Current Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // Modifica la posizione Y del titolo rispetto all'area del grafico
            chart.Title.YRatioToChart = 0.1; // 10% from top of chart area
            
            // Visualizza il nuovo valore YRatioToChart
            Console.WriteLine("New Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // Accedi alla legenda che eredita anche da ChartFrame
            chart.Legend.Position = LegendPositionType.Top;
            
            // Visualizza il valore corrente YRatioToChart per la legenda
            Console.WriteLine("Current Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // Modifica la posizione Y della legenda rispetto all'area del grafico
            chart.Legend.YRatioToChart = 0.15; // 15% from top of chart area
            
            // Visualizza il nuovo valore YRatioToChart per la legenda
            Console.WriteLine("New Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // Salva la cartella di lavoro
            workbook.Save("ChartFramePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


