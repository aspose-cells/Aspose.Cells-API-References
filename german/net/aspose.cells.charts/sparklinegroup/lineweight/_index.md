---
title: "SparklineGroup.LineWeight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroup-Eigenschaft. Gibt die Linienstärke jeder Linien‑Sparkline in der Sparkline-Gruppe in Punkt zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.charts/sparklinegroup/lineweight/
---
## SparklineGroup.LineWeight property

Liest und legt die Linienstärke jeder Linien‑Sparkline in der Sparkline-Gruppe in Punkt als Einheit fest.

```csharp
public double LineWeight { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyLineWeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Sparkline-Gruppe erstellen
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // LineWeight-Eigenschaft festlegen
            group.LineWeight = 2.5; // Thicker line weight for visibility

            workbook.Save("SparklineLineWeightDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


