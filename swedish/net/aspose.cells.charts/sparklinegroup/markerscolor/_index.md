---
title: "SparklineGroup.MarkersColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup-egenskap. Hämtar och anger färgen på punkterna i varje linjesparkline i sparkline-gruppen"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/markerscolor/
---
## SparklineGroup.MarkersColor property

Hämtar och anger färgen på punkterna i varje linjesparkline i sparkline-gruppen.

```csharp
public CellsColor MarkersColor { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyMarkersColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Exempeldata
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

            // Konfigurera sparkline-utseende
            group.ShowMarkers = true;
            CellsColor markersColor = workbook.CreateCellsColor();
            markersColor.Color = Color.Black;
            group.MarkersColor = markersColor;

            // Spara arbetsboken
            workbook.Save("SparklineMarkersColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


