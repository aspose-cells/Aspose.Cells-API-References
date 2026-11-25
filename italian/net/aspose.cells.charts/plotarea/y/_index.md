---
title: "PlotArea.Y"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PlotArea. Restituisce o imposta la coordinata y dell'angolo superiore del riquadro di delimitazione dell'area del grafico in unità di 1/4000 dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/plotarea/y/
---
## PlotArea.Y property

Restituisce o imposta la coordinata y dell'angolo superiore del riquadro di delimitazione dell'area del grafico in unità di 1/4000 dell'area del grafico.

```csharp
[Obsolete("Use PlotArea.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```

### Osservazioni

Il riquadro di delimitazione dell'area del grafico include l'area del grafico, le tacche (etichette delle tacche) e un piccolo bordo attorno alle tacche. Se il valore non è stato creato da MS Excel, si prega di chiamare il metodo Chart.Calculate() prima di chiamare questo metodo.

Le **X**, **Y**, **Width** e **Height** di **PlotArea** rappresentano il riquadro delimitante dell'area del grafico che include l'area del grafico, le tacche (etichette delle tacche) e un piccolo bordo attorno alle tacche. Se vuoi ottenere le dimensioni reali dell'area del grafico, dovresti chiamare le proprietà **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** e **InnerHeightRatioToChart**.

Per Excel 2007 o versioni successive, il valore predefinito è zero. Dovresti ottenere il valore dopo aver chiamato Chart.Calculate().

Nota: quando Y è impostato, la proprietà **IsInnerMode** verrà impostata automaticamente a false.

NOTA: questo membro è ora obsoleto. Si prega di utilizzare la proprietà **PlotArea.YRatioToChart**, invece. Y = YRatioToChart * 4000. Questa proprietà sarà rimossa 12 mesi dopo, a partire da febbraio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PlotAreaPropertyYDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Dati di esempio
            sheet.Cells["A1"].PutValue("Category 1");
            sheet.Cells["A2"].PutValue("Category 2");
            sheet.Cells["B1"].PutValue(100);
            sheet.Cells["B2"].PutValue(50);

            // Crea grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Imposta i dati del grafico
            chart.NSeries.Add("B1:B2", false);
            chart.NSeries.CategoryData = "A1:A2";

            // Configura l'area del grafico
            chart.PlotArea.Width = 300;
            chart.PlotArea.Height = 200;
            chart.PlotArea.X = 100;
            chart.PlotArea.Y = 150; // Demonstrating Y property usage

            // Salva la cartella di lavoro
            workbook.Save("PlotAreaPropertyYDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


