---
title: "PlotArea.InnerYRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PlotArea. Ottiene o imposta la coordinata x dell'angolo superiore sinistro dell'area del grafico in unità del rapporto dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/plotarea/inneryratiotochart/
---
## PlotArea.InnerYRatioToChart property

Ottiene o ottiene la coordinata x dell'angolo superiore superiore dell'area del grafico in unità del rapporto dell'area del diagramma.

```csharp
public double InnerYRatioToChart { get; set; }
```

### Osservazioni

Il riquadro di delimitazione dell'area del grafico include l'area del grafico, le tacche (etichette delle tacche) e un piccolo bordo attorno alle tacche. Se il valore non è stato creato da MS Excel, si prega di chiamare il metodo Chart.Calculate() prima di chiamare questo metodo.

Le **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** e **HeightRatioToChart** di **PlotArea** rappresentano il riquadro delimitante dell'area del grafico che include l'area del grafico, le tacche (etichette delle tacche) e un piccolo bordo attorno alle tacche. Se vuoi ottenere le dimensioni reali dell'area del grafico, dovresti chiamare le proprietà **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** e **InnerHeightRatioToChart**.

Per Excel 2007 o versioni successive, il valore predefinito è zero. Dovresti ottenere il valore dopo aver chiamato Chart.Calculate().

InnerY in pixel = InnerYRatioToChart * chart.ChartObject.Width. Nota: quando InnerYRatioToChart è impostato, la proprietà IsInnerMode verrà impostata automaticamente su True.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyInnerYRatioToChartDemo
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

            // Ottieni l'area del grafico
            PlotArea plotArea = chart.PlotArea;

            // Visualizza il valore corrente di InnerYRatioToChart
            Console.WriteLine("Current InnerYRatioToChart value: " + plotArea.InnerYRatioToChart);

            // Modifica il valore di InnerYRatioToChart (da 0,0 a 1,0 rappresenta dallo 0% al 100% dell'area del grafico)
            plotArea.InnerYRatioToChart = 0.2;

            // Visualizza il nuovo valore
            Console.WriteLine("New InnerYRatioToChart value: " + plotArea.InnerYRatioToChart);

            // Salva la cartella di lavoro
            workbook.Save("PlotAreaPropertyInnerYRatioToChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


