---
title: "SparklineGroup.ShowHighPoint"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup-egenskap. Anger om de högsta datapunkterna i sparkline-gruppen ska markeras"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/showhighpoint/
---
## SparklineGroup.ShowHighPoint property

Anger om de högsta datapunkterna i sparkline-gruppen ska markeras.

```csharp
public bool ShowHighPoint { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowHighPointDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempeldata
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Skapa sparkline-grupp
            CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Lägg till sparkline
            group.Sparklines.Add("A1:D1", 0, 4);

            // Konfigurera visning av högsta punkten
            group.ShowHighPoint = true;
            CellsColor highColor = workbook.CreateCellsColor();
            highColor.Color = System.Drawing.Color.Green;
            group.HighPointColor = highColor;

            // Spara arbetsbok
            workbook.Save("SparklineHighPointDemo.xlsx");
        }
    }
}
```

### Se även

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


