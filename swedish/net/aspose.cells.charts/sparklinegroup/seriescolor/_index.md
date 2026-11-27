---
title: "SparklineGroup.SeriesColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup egenskap. Hämtar och anger färgen på sparklines i sparkline-gruppen"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/seriescolor/
---
## SparklineGroup.SeriesColor property

Hämtar och anger färgen på sparkline-diagrammen i sparkline-gruppen.

```csharp
public CellsColor SeriesColor { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertySeriesColorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Exempeldata
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(8);
            ws.Cells["A3"].PutValue(3);
            
            // Skapa sparkline-grupp
            CellArea dataRange = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            CellArea locationRange = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 1, EndColumn = 1 };
            int index = ws.SparklineGroups.Add(SparklineType.Column, "A1:A3", false, locationRange);
            
            // Ställ in seriefärg
            SparklineGroup group = ws.SparklineGroups[index];
            CellsColor color = wb.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;
            
            wb.Save("SparklineSeriesColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


