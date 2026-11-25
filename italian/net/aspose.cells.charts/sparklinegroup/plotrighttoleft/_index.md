---
title: "SparklineGroup.PlotRightToLeft"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Indica se i dati del grafico sono da destra a sinistra"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/plotrighttoleft/
---
## SparklineGroup.PlotRightToLeft property

Indica se i dati del grafico sono da destra a sinistra.

```csharp
public bool PlotRightToLeft { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyPlotRightToLeftDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Crea gruppo sparkline
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Aggiungi sparkline
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Imposta i colori delle sparklines
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;

            // Dimostra la proprietà PlotRightToLeft
            group.PlotRightToLeft = true; // Plot data points from right to left

            // Salva la cartella di lavoro
            workbook.Save("SparklineRightToLeftDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


