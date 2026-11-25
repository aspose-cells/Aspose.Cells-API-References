---
title: "PlotArea.WidthRatioToChart"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PlotArea. Ottiene o imposta la larghezza del riquadro delimitante dell'area del grafico in unità del rapporto con l'area del diagramma"
type: docs
url: /it/net/aspose.cells.charts/plotarea/widthratiotochart/
---
## PlotArea.WidthRatioToChart property

Ottiene o imposta la larghezza del riquadro di delimitazione dell'area del grafico in unità del rapporto dell'area del diagramma.

```csharp
public override double WidthRatioToChart { get; set; }
```

### Osservazioni

Il riquadro di delimitazione dell'area del grafico include l'area del grafico, le tacche (etichette delle tacche) e un piccolo bordo attorno alle tacche. Se il valore non è stato creato da MS Excel, si prega di chiamare il metodo Chart.Calculate() prima di chiamare questo metodo.

Le **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** e **HeightRatioToChart** di **PlotArea** rappresentano il riquadro delimitante dell'area del grafico che include l'area del grafico, le tacche (etichette delle tacche) e un piccolo bordo attorno alle tacche. Se vuoi ottenere le dimensioni reali dell'area del grafico, dovresti chiamare le proprietà **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** e **InnerHeightRatioToChart**.

Per Excel 2007 o versioni successive, il valore predefinito è zero. Dovresti ottenere il valore dopo aver chiamato Chart.Calculate().

WidthPixel = WidthRatioToChart * chart.ChartObject.Width. Nota: Quando WidthRatioToChart è impostato, la proprietà IsInnerMode verrà impostata automaticamente su false.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyWidthRatioToChartDemo
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

            // Aggiungi un grafico e ottieni la sua area del grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            PlotArea plotArea = chart.PlotArea;

            // Mostra il valore corrente di WidthRatioToChart
            Console.WriteLine("Current WidthRatioToChart value: " + plotArea.WidthRatioToChart);

            // Modifica il rapporto di larghezza e vedi l'effetto
            plotArea.WidthRatioToChart = 0.6; // 60% of chart width
            Console.WriteLine("WidthRatioToChart changed to: " + plotArea.WidthRatioToChart);

            // Salva la cartella di lavoro
            workbook.Save("PlotAreaWidthRatioToChartDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


