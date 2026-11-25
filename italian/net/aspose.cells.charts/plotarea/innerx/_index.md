---
title: "PlotArea.InnerX"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PlotArea. Ottiene o imposta la coordinata x dell'angolo superiore sinistro dell'area del grafico in unità di 1/4000 dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/plotarea/innerx/
---
## PlotArea.InnerX property

Ottiene o imposta la coordinata x dell'angolo superiore sinistro dell'area del grafico in unità di 1/4000 dell'area del grafico.

```csharp
[Obsolete("Use PlotArea.InnerXRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int InnerX { get; set; }
```

### Osservazioni

Il riquadro di delimitazione dell'area del grafico include l'area del grafico, le tacche (etichette delle tacche) e un piccolo bordo attorno alle tacche. Se il valore non è stato creato da MS Excel, si prega di chiamare il metodo Chart.Calculate() prima di chiamare questo metodo.

Le **X**, **Y**, **Width** e **Height** di **PlotArea** rappresentano il riquadro delimitante dell'area del grafico che include l'area del grafico, le tacche (etichette delle tacche) e un piccolo bordo attorno alle tacche. Se vuoi ottenere le dimensioni reali dell'area del grafico, dovresti chiamare le proprietà **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** e **InnerHeightRatioToChart**.

Per Excel 2007 o versioni successive, il valore predefinito è zero. Dovresti ottenere il valore dopo aver chiamato Chart.Calculate().

Nota: quando InnerX è impostato, la proprietà IsInnerMode verrà impostata automaticamente su True.

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà PlotArea.InnerXRatioToChart, invece. InnerX = InnerXRatioToChart * 4000. Questa proprietà sarà rimossa 12 mesi dopo, a partire da febbraio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyInnerXDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Imposta i dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configura l'area del grafico
            Aspose.Cells.Charts.PlotArea plotArea = chart.PlotArea;
            plotArea.InnerX = 200; // Demonstrate InnerX property
            plotArea.InnerY = 100;
            plotArea.InnerWidth = 2800;
            plotArea.InnerHeight = 1800;

            workbook.Save("PlotAreaInnerXDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


