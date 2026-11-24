---
title: "SparklineGroup.PlotRightToLeft"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroup-Eigenschaft. Gibt an, ob die Daten von rechts nach links dargestellt werden"
type: docs
url: /de/net/aspose.cells.charts/sparklinegroup/plotrighttoleft/
---
## SparklineGroup.PlotRightToLeft property

Gibt an, ob die Plot-Daten von rechts nach links verlaufen.

```csharp
public bool PlotRightToLeft { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyPlotRightToLeftDemo
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

            // Sparkline-Gruppe erstellen
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Sparkline hinzufügen
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Sparkline-Farben festlegen
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;

            // PlotRightToLeft-Eigenschaft demonstrieren
            group.PlotRightToLeft = true; // Plot data points from right to left

            // Speichere die Arbeitsmappe
            workbook.Save("SparklineRightToLeftDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


