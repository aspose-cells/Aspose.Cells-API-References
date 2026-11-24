---
title: "SparklineGroup.ShowHorizontalAxis"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroup-Eigenschaft. Gibt an, ob die horizontale Achse der Sparkline angezeigt wird. Die horizontale Achse erscheint, wenn die Sparkline Daten enthält, die die Nullachse überschreiten"
type: docs
url: /de/net/aspose.cells.charts/sparklinegroup/showhorizontalaxis/
---
## SparklineGroup.ShowHorizontalAxis property

Gibt an, ob die horizontale Achse der Sparkline angezeigt werden soll. Die horizontale Achse erscheint, wenn die Sparkline Daten enthält, die die Nullachse überschreiten.

```csharp
public bool ShowHorizontalAxis { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowHorizontalAxisDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Sparkline-Position definieren
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Sparkline-Gruppe hinzufügen
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Sparkline-Eigenschaften konfigurieren
            group.ShowHorizontalAxis = true;
            CellsColor axisColor = workbook.CreateCellsColor();
            axisColor.Color = Color.Gray;
            group.HorizontalAxisColor = axisColor;

            // Speichere die Arbeitsmappe
            workbook.Save("SparklineWithHorizontalAxis.xlsx");
        }
    }
}
```

### Siehe auch

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


