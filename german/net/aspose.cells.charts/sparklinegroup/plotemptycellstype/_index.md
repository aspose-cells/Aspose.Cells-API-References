---
title: "SparklineGroup.PlotEmptyCellsType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroup-Eigenschaft. Gibt an, wie leere Zellen dargestellt werden"
type: docs
url: /de/net/aspose.cells.charts/sparklinegroup/plotemptycellstype/
---
## SparklineGroup.PlotEmptyCellsType property

Gibt an, wie leere Zellen dargestellt werden.

```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Daten mit einigen leeren Zellen hinzufügen
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(null); // Empty cell
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Definiert den CellArea für die Sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Eine Sparkline-Gruppe hinzufügen
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Festlegen, wie leere Zellen dargestellt werden sollen
            group.PlotEmptyCellsType = PlotEmptyCellsType.Zero;

            // Sparkline zur Gruppe hinzufügen
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Speichere die Arbeitsmappe
            workbook.Save("SparklineEmptyCellsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


