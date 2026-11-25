---
title: "PlotArea.InnerY"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PlotArea. Ottiene o imposta la coordinata x dell'angolo superiore dell'area del grafico in unità di 1/4000 dell'area del diagramma"
type: docs
url: /it/net/aspose.cells.charts/plotarea/innery/
---
## PlotArea.InnerY property

Ottiene o imposta la coordinata x dell'angolo superiore dell'area del grafico in unità di 1/4000 dell'area del diagramma.

```csharp
[Obsolete("Use PlotArea.InnerYRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerY { get; set; }
```

### Osservazioni

Il riquadro di delimitazione dell'area del grafico include l'area del grafico, le tacche (etichette delle tacche) e un piccolo bordo attorno alle tacche. Se il valore non è stato creato da MS Excel, si prega di chiamare il metodo Chart.Calculate() prima di chiamare questo metodo.

Le **X**, **Y**, **Width** e **Height** di **PlotArea** rappresentano il riquadro delimitante dell'area del grafico che include l'area del grafico, le tacche (etichette delle tacche) e un piccolo bordo attorno alle tacche. Se vuoi ottenere le dimensioni reali dell'area del grafico, dovresti chiamare le proprietà **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** e **InnerHeightRatioToChart**.

Per Excel 2007 o versioni successive, il valore predefinito è zero. Dovresti ottenere il valore dopo aver chiamato Chart.Calculate().

Nota: Quando InnerY è impostato, la proprietà IsInnerMode verrà impostata automaticamente su True.

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà PlotArea.InnerYRatioToChart, invece. InnerY = InnerYRatioToChart * 4000. Questa proprietà sarà rimossa 12 mesi dopo, a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyInnerYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configura l'area del grafico con InnerY
            PlotArea plotArea = chart.PlotArea;
            plotArea.InnerY = 200;
            plotArea.InnerHeight = 1800;
            plotArea.IsInnerMode = true;

            workbook.Save("PlotAreaInnerYDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


