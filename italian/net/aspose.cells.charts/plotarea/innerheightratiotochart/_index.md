---
title: "PlotArea.InnerHeightRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PlotArea. Ottiene o imposta l'altezza dell'area del grafico in unità del rapporto dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/plotarea/innerheightratiotochart/
---
## PlotArea.InnerHeightRatioToChart property

Ottiene o imposta l'altezza dell'area del grafico in unità del rapporto dell'area del diagramma.

```csharp
public double InnerHeightRatioToChart { get; set; }
```

### Osservazioni

Il riquadro di delimitazione dell'area del grafico include l'area del grafico, le tacche (etichette delle tacche) e un piccolo bordo attorno alle tacche. Se il valore non è stato creato da MS Excel, si prega di chiamare il metodo Chart.Calculate() prima di chiamare questo metodo.

Le **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** e **HeightRatioToChart** di **PlotArea** rappresentano il riquadro delimitante dell'area del grafico che include l'area del grafico, le tacche (etichette delle tacche) e un piccolo bordo attorno alle tacche. Se vuoi ottenere le dimensioni reali dell'area del grafico, dovresti chiamare le proprietà **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** e **InnerHeightRatioToChart**.

Per Excel 2007 o versioni successive, il valore predefinito è zero. Dovresti ottenere il valore dopo aver chiamato Chart.Calculate().

InnerHeight in pixel = InnerXRatioToChart * chart.ChartObject.Width. Nota: quando InnerHeightRatioToChart è impostato, la proprietà **IsInnerMode** verrà impostata automaticamente a True.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyInnerHeightRatioToChartDemo
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

            // Accedi all'area del grafico
            PlotArea plotArea = chart.PlotArea;

            // Visualizza il valore corrente di InnerHeightRatioToChart
            Console.WriteLine("Current InnerHeightRatioToChart value: " + plotArea.InnerHeightRatioToChart);

            // Imposta un nuovo valore per InnerHeightRatioToChart (0.5 = 50% dell'altezza dell'area del grafico)
            plotArea.InnerHeightRatioToChart = 0.5;

            // Dimostra l'effetto salvando la cartella di lavoro
            workbook.Save("PlotAreaInnerHeightRatioToChartDemo.xlsx");

            // Mostra il nuovo valore
            Console.WriteLine("New InnerHeightRatioToChart value: " + plotArea.InnerHeightRatioToChart);
        }
    }
}
```

### Vedi anche

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


