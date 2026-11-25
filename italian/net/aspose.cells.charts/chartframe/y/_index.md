---
title: "ChartFrame.Y"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Ottiene o imposta la coordinata y dell'angolo superiore sinistro in unità di 1/4000 dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartframe/y/
---
## ChartFrame.Y property

Ottiene o imposta la coordinata y dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico.

```csharp
[Obsolete("Use ChartFrame.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Y { get; set; }
```

### Osservazioni

Come convertire le unità di 1/4000 in pixel? Y in pixel = Y * Chart.ChartObject.Height / 4000d;

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.YRatioToChart, invece. Y = YRatioToChart * 4000. Questa proprietà sarà rimossa tra 12 mesi a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyYDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["A2"].PutValue("A");
            cells["A3"].PutValue("B");
            cells["A4"].PutValue("C");
            cells["B1"].PutValue("Value");
            cells["B2"].PutValue(10);
            cells["B3"].PutValue(20);
            cells["B4"].PutValue(30);

            // Aggiungi grafico
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Accedi al titolo del grafico e imposta la posizione Y
            chart.Title.Text = "Sample Chart";
            chart.Title.Y = 1000; // Demonstrate Y property usage

            // Salva la cartella di lavoro
            workbook.Save("ChartFramePropertyYDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


