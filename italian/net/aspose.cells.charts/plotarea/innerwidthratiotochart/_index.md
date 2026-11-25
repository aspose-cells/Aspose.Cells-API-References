---
title: "PlotArea.InnerWidthRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PlotArea. Ottiene o imposta la larghezza dell'area del grafico in unità del rapporto dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/plotarea/innerwidthratiotochart/
---
## PlotArea.InnerWidthRatioToChart property

Ottiene o imposta la larghezza dell'area del grafico in unità del rapporto dell'area del diagramma.

```csharp
public double InnerWidthRatioToChart { get; set; }
```

### Osservazioni

Il riquadro di delimitazione dell'area del grafico include l'area del grafico, le tacche (etichette delle tacche) e un piccolo bordo attorno alle tacche. Se il valore non è stato creato da MS Excel, si prega di chiamare il metodo Chart.Calculate() prima di chiamare questo metodo.

Le **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** e **HeightRatioToChart** di **PlotArea** rappresentano il riquadro delimitante dell'area del grafico che include l'area del grafico, le tacche (etichette delle tacche) e un piccolo bordo attorno alle tacche. Se vuoi ottenere le dimensioni reali dell'area del grafico, dovresti chiamare le proprietà **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** e **InnerHeightRatioToChart**.

Per Excel 2007 o versioni successive, il valore predefinito è zero. Dovresti ottenere il valore dopo aver chiamato Chart.Calculate().

InnerWidth in pixel = InnerXRatioToChart * chart.ChartObject.Width. Nota: quando InnerWidthRatioToChart è impostato, la proprietà IsInnerMode verrà impostata automaticamente su True.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyInnerWidthRatioToChartDemo
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
            
            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Accedi all'area del grafico
            PlotArea plotArea = chart.PlotArea;
            
            // Visualizza il valore corrente di InnerWidthRatioToChart
            Console.WriteLine("Current InnerWidthRatioToChart value: " + plotArea.InnerWidthRatioToChart);
            
            // Imposta un nuovo valore per InnerWidthRatioToChart (0,5 significa il 50% della larghezza del grafico)
            plotArea.InnerWidthRatioToChart = 0.5;
            
            // Mostra l'effetto della modifica
            Console.WriteLine("Plot area width changed to 50% of chart width");
            
            // Salva il risultato
            workbook.Save("PlotAreaPropertyInnerWidthRatioToChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


