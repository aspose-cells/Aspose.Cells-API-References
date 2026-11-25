---
title: "SparklineGroup.PlotEmptyCellsType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Indica come tracciare le celle vuote"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/plotemptycellstype/
---
## SparklineGroup.PlotEmptyCellsType property

Indica come tracciare le celle vuote.

```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyPlotEmptyCellsTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati con alcune celle vuote
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(null); // Empty cell
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Definisci il CellArea per lo sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Aggiungi un gruppo sparkline
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Imposta come le celle vuote devono essere tracciate
            group.PlotEmptyCellsType = PlotEmptyCellsType.Zero;

            // Aggiungi la sparkline al gruppo
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Salva la cartella di lavoro
            workbook.Save("SparklineEmptyCellsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


