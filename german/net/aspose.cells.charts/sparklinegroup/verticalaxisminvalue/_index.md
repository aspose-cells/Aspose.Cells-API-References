---
title: "SparklineGroup.VerticalAxisMinValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroup-Eigenschaft. Gibt den benutzerdefinierten Minimalwert für die vertikale Achse zurück und legt ihn fest."
type: docs
url: /de/net/aspose.cells.charts/sparklinegroup/verticalaxisminvalue/
---
## SparklineGroup.VerticalAxisMinValue property

Liest und setzt den benutzerdefinierten Minimalwert für die vertikale Achse.

```csharp
public double VerticalAxisMinValue { get; set; }
```

### Hinweise

Wenn diese Eigenschaft gesetzt ist, wird [`VerticalAxisMinValueType`](../verticalaxisminvaluetype/) auf Custom gesetzt.

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMinValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(2);
            sheet.Cells["A3"].PutValue(1);
            sheet.Cells["A4"].PutValue(3);

            // Sparkline-Gruppe erstellen
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 3;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A4", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Vertikalen Achsen-Minimalwert festlegen
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.Custom;
            group.VerticalAxisMinValue = 0.0;

            // Speichere die Arbeitsmappe
            workbook.Save("SparklineVerticalAxisMinValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


