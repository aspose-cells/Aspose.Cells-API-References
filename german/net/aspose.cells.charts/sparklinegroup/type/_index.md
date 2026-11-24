---
title: "SparklineGroup.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroup-Eigenschaft. Gibt den Sparkline-Typ der Sparkline-Gruppe an"
type: docs
url: /de/net/aspose.cells.charts/sparklinegroup/type/
---
## SparklineGroup.Type property

Gibt den Sparkline-Typ der Sparkline-Gruppe an.

```csharp
public SparklineType Type { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyTypeDemo
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

            // Sparkline-Gruppe mit Spaltentyp erstellen
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Column, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Den Sparkline-Typ zu Linie ändern
            group.Type = SparklineType.Line;

            // Sparkline zur Gruppe hinzufügen
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Speichere die Arbeitsmappe
            workbook.Save("SparklineTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


