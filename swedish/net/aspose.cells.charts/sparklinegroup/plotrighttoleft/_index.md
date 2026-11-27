---
title: "SparklineGroup.PlotRightToLeft"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup-egenskap. Anger om plottdatan är från höger till vänster"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/plotrighttoleft/
---
## SparklineGroup.PlotRightToLeft property

Anger om plottdatan är från höger till vänster.

```csharp
public bool PlotRightToLeft { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Skapa sparkline-grupp
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Lägg till sparkline
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Ange sparkline-färger
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;

            // Demonstrera PlotRightToLeft-egenskapen
            group.PlotRightToLeft = true; // Plot data points from right to left

            // Spara arbetsboken
            workbook.Save("SparklineRightToLeftDemo.xlsx");
        }
    }
}
```

### Se även

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


