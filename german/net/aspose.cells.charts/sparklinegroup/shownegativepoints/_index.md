---
title: "SparklineGroup.ShowNegativePoints"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroup-Eigenschaft. Gibt an, ob die negativen Werte in der Sparkline-Gruppe mit einer anderen Farbe oder einem anderen Marker hervorgehoben werden sollen."
type: docs
url: /de/net/aspose.cells.charts/sparklinegroup/shownegativepoints/
---
## SparklineGroup.ShowNegativePoints property

Gibt an, ob die negativen Werte in der Sparkline-Gruppe mit einer anderen Farbe oder einem anderen Marker hervorgehoben werden sollen.

```csharp
public bool ShowNegativePoints { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowNegativePointsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Daten mit negativen Werten hinzufügen, um ShowNegativePoints zu demonstrieren
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(-2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(-3);

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

            // Sparkline-Gruppeneigenschaften konfigurieren
            group.ShowNegativePoints = true;
            CellsColor negativePointsColor = workbook.CreateCellsColor();
            negativePointsColor.Color = Color.Blue;
            group.NegativePointsColor = negativePointsColor;

            // Speichere die Arbeitsmappe
            workbook.Save("SparklineNegativePointsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


