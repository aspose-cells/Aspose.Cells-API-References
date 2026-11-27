---
title: "SparklineGroup.ShowLastPoint"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup-egenskap. Anger om den sista datapunkten i sparkline-gruppen ska markeras"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/showlastpoint/
---
## SparklineGroup.ShowLastPoint property

Anger om den sista datapunkten i sparkline-gruppen ska markeras.

```csharp
public bool ShowLastPoint { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowLastPointDemo
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

            // Konfigurera sparkline-utseende
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;
            group.LineWeight = 1.0;

            // Aktivera och färga den sista punkten
            group.ShowLastPoint = true;
            CellsColor lastPointColor = workbook.CreateCellsColor();
            lastPointColor.Color = Color.Yellow;
            group.LastPointColor = lastPointColor;

            // Spara arbetsboken
            workbook.Save("SparklineShowLastPointDemo.xlsx");
        }
    }
}
```

### Se även

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


