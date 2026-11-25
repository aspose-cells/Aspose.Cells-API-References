---
title: "PlotArea.XRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PlotArea. Ottiene o imposta la coordinata x dell'angolo superiore sinistro del riquadro delimitante dell'area del grafico come rapporto dell'area del diagramma"
type: docs
url: /it/net/aspose.cells.charts/plotarea/xratiotochart/
---
## PlotArea.XRatioToChart property

Ottiene o imposta la coordinata x dell'angolo superiore sinistro del riquadro di delimitazione dell'area del grafico come rapporto dell'area del diagramma.

```csharp
public override double XRatioToChart { get; set; }
```

### Osservazioni

Il riquadro di delimitazione dell'area del grafico include l'area del grafico, le tacche (etichette delle tacche) e un piccolo bordo attorno alle tacche. Se il valore non è stato creato da MS Excel, si prega di chiamare il metodo Chart.Calculate() prima di chiamare questo metodo.

Le **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** e **HeightRatioToChart** di **PlotArea** rappresentano il riquadro delimitante dell'area del grafico che include l'area del grafico, le tacche (etichette delle tacche) e un piccolo bordo attorno alle tacche. Se vuoi ottenere le dimensioni reali dell'area del grafico, dovresti chiamare le proprietà **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** e **InnerHeightRatioToChart**.

Per Excel 2007 o versioni successive, il valore predefinito è zero. Dovresti ottenere il valore dopo aver chiamato Chart.Calculate().

XPixel = XRatioToChart * chart.ChartObject.Width. Nota: Quando XRatioToChart è impostato, la proprietà IsInnerMode verrà impostata automaticamente su false.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyXRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Ottieni l'area del grafico
            PlotArea plotArea = chart.PlotArea;

            // Visualizza il valore corrente di XRatioToChart
            Console.WriteLine("Current XRatioToChart value: " + plotArea.XRatioToChart);

            // Modifica il valore XRatioToChart per spostare l'area del grafico orizzontalmente
            plotArea.XRatioToChart = 0.2; // 20% from the left of the chart area

            // Visualizza il nuovo valore di XRatioToChart
            Console.WriteLine("New XRatioToChart value: " + plotArea.XRatioToChart);

            // Salva la cartella di lavoro per vedere l'effetto
            workbook.Save("PlotAreaXRatioToChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


