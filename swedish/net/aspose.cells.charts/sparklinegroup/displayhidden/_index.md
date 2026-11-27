---
title: "SparklineGroup.DisplayHidden"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup egenskap. Anger om data i dolda rader och kolumner ska visas"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/displayhidden/
---
## SparklineGroup.DisplayHidden property

Indikerar om data ska visas i dolda rader och kolumner.

```csharp
public bool DisplayHidden { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyDisplayHiddenDemo
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

            // Definiera sparkline-plats
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Lägg till sparkline-grupp
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Lägg till sparkline i gruppen
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Konfigurera sparkline-utseende
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Blue;
            group.SeriesColor = seriesColor;

            // Demonstrera DisplayHidden-egenskapen
            group.DisplayHidden = true; // Show sparklines for hidden data

            // Spara arbetsboken
            workbook.Save("SparklineDisplayHiddenDemo.xlsx");
        }
    }
}
```

### Se även

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


