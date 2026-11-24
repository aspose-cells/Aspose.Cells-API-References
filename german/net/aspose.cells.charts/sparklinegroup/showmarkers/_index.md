---
title: "SparklineGroup.ShowMarkers"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroup-Eigenschaft. Gibt an, ob jeder Punkt in jeder Linien‑Sparkline der Sparkline‑Gruppe hervorgehoben werden soll."
type: docs
url: /de/net/aspose.cells.charts/sparklinegroup/showmarkers/
---
## SparklineGroup.ShowMarkers property

Gibt an, ob jeder Punkt in jeder Linien‑Sparkline der Sparkline-Gruppe hervorgehoben werden soll.

```csharp
public bool ShowMarkers { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowMarkersDemo
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

            // Sparkline hinzufügen
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Aussehen der Sparkline konfigurieren
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;

            group.ShowMarkers = true;
            
            CellsColor markersColor = workbook.CreateCellsColor();
            markersColor.Color = Color.Black;
            group.MarkersColor = markersColor;

            // Speichere die Arbeitsmappe
            workbook.Save("SparklineWithMarkers.xlsx");
        }
    }
}
```

### Siehe auch

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


