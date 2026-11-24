---
title: "SparklineGroup.VerticalAxisMaxValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroup-Eigenschaft. Gibt den benutzerdefinierten Maximalwert für die vertikale Achse zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.charts/sparklinegroup/verticalaxismaxvalue/
---
## SparklineGroup.VerticalAxisMaxValue property

Liest und setzt den benutzerdefinierten Maximalwert für die vertikale Achse.

```csharp
public double VerticalAxisMaxValue { get; set; }
```

### Hinweise

Wenn diese Eigenschaft gesetzt ist, wird [`VerticalAxisMaxValueType`](../verticalaxismaxvaluetype/) auf Custom gesetzt.

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMaxValueDemo
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

            // Vertikalen Achsen-Maximalwert festlegen
            group.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Custom;
            group.VerticalAxisMaxValue = 10.0;

            // Speichere die Arbeitsmappe
            workbook.Save("SparklineVerticalAxisMaxValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


