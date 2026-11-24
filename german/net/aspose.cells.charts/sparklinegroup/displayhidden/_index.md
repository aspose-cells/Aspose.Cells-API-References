---
title: "SparklineGroup.DisplayHidden"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroup-Eigenschaft. Gibt an, ob Daten in ausgeblendeten Zeilen und Spalten angezeigt werden sollen."
type: docs
url: /de/net/aspose.cells.charts/sparklinegroup/displayhidden/
---
## SparklineGroup.DisplayHidden property

Gibt an, ob Daten in ausgeblendeten Zeilen und Spalten angezeigt werden.

```csharp
public bool DisplayHidden { get; set; }
```

### Beispiele

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

            // Sparkline zur Gruppe hinzufügen
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Aussehen der Sparkline konfigurieren
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Blue;
            group.SeriesColor = seriesColor;

            // DisplayHidden-Eigenschaft demonstrieren
            group.DisplayHidden = true; // Show sparklines for hidden data

            // Speichere die Arbeitsmappe
            workbook.Save("SparklineDisplayHiddenDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


