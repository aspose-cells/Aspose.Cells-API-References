---
title: "SparklineGroup.PlotEmptyCellsType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup-egenskap. Anger hur tomma celler ska plottas"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/plotemptycellstype/
---
## SparklineGroup.PlotEmptyCellsType property

Anger hur tomma celler ska plottas.

```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till data med några tomma celler
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(null); // Empty cell
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Definiera CellArea för sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Lägg till en sparkline-grupp
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Ange hur tomma celler ska plottas
            group.PlotEmptyCellsType = PlotEmptyCellsType.Zero;

            // Lägg till sparkline i gruppen
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Spara arbetsboken
            workbook.Save("SparklineEmptyCellsDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


