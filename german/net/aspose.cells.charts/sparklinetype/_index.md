---
title: "Enum SparklineType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.SparklineType enum. Stellt die Sparkline-Typen dar"
type: docs
url: /de/net/aspose.cells.charts/sparklinetype/
---
## SparklineType enumeration

Stellt die Sparkline‑Typen dar.

```csharp
public enum SparklineType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Line | `0` | Linien-Sparkline. |
| Column | `1` | Spalten-Sparkline. |
| Stacked | `2` | Stellt eine Gewinn/Verlust-Sparkline dar. |
| WinLoss | `2` | Stellt eine Gewinn/Verlust-Sparkline dar. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineTypeDemo
    {
        public static void SparklineTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Definiert den CellArea für die Sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Fügt der Arbeitsmappe eine Sparkline-Gruppe hinzu
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];

            // Fügt der Gruppe Sparklines hinzu
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Sparkline-Gruppe anpassen
            CellsColor clr = workbook.CreateCellsColor();
            clr.Color = Color.Orange;
            group.SeriesColor = clr;

            // Setze die hohen Punkte auf Grün und die niedrigen Punkte auf Rot
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            group.HighPointColor.Color = Color.Green;
            group.LowPointColor.Color = Color.Red;

            // Linienstärke festlegen
            group.LineWeight = 1.0;

            // Speichere die Arbeitsmappe
            workbook.Save("SparklineTypeExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


