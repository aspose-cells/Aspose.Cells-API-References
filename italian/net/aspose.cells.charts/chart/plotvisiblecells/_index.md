---
title: "Chart.PlotVisibleCells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Indica se tracciare solo le celle visibili"
type: docs
url: /it/net/aspose.cells.charts/chart/plotvisiblecells/
---
## Chart.PlotVisibleCells property

Indica se tracciare solo le celle visibili.

```csharp
[Obsolete("Use PlotVisibleCellsOnly property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool PlotVisibleCells { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, utilizza la proprietà PlotVisibleCellsOnly. Questo metodo sarà rimosso 12 mesi dopo, a partire da dicembre 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotVisibleCellsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("Alice");
            worksheet.Cells["A3"].PutValue("Bob");
            worksheet.Cells["A4"].PutValue("Eve");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(90);
            worksheet.Cells["B3"].PutValue(85);
            worksheet.Cells["B4"].PutValue(95);

            // Nascondi alcune righe
            worksheet.Cells.HideRow(2);
            worksheet.Cells.HideRow(3);

            // Crea grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Dimostra la proprietà PlotVisibleCells
            chart.PlotVisibleCells = false; // Will not plot hidden cells
            // chart.PlotVisibleCells = true; // Traccerà le celle nascoste (commentato per la demo)

            // Salva la cartella di lavoro
            workbook.Save("ChartPlotVisibleCellsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


