---
title: "SparklineGroup.HorizontalAxisDateRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroup-Eigenschaft. Stellt den Bereich dar, der die Datumswerte für die Sparkline-Daten enthält."
type: docs
url: /de/net/aspose.cells.charts/sparklinegroup/horizontalaxisdaterange/
---
## SparklineGroup.HorizontalAxisDateRange property

Stellt den Bereich dar, der die Datumswerte für die Sparkline-Daten enthält.

```csharp
public string HorizontalAxisDateRange { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyHorizontalAxisDateRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Datum- und Wertdaten für die Sparkline hinzufügen
            sheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1));
            sheet.Cells["B1"].PutValue(new DateTime(2023, 2, 1));
            sheet.Cells["C1"].PutValue(new DateTime(2023, 3, 1));
            sheet.Cells["D1"].PutValue(new DateTime(2023, 4, 1));
            
            sheet.Cells["A2"].PutValue(5);
            sheet.Cells["B2"].PutValue(2);
            sheet.Cells["C2"].PutValue(1);
            sheet.Cells["D2"].PutValue(3);

            // Definieren Sie den Zellbereich, in dem die Sparkline platziert wird
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 1,
                EndRow = 1
            };

            // Eine Sparkline-Gruppe mit Datumsachse hinzufügen
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A2:D2", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            
            // Datumsbereich für die horizontale Achse festlegen
            group.HorizontalAxisDateRange = "A1:D1";
            group.ShowHorizontalAxis = true;

            // Speichere die Arbeitsmappe
            workbook.Save("SparklineWithDateAxis.xlsx");
        }
    }
}
```

### Siehe auch

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


