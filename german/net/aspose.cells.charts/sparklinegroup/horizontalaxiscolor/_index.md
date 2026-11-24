---
title: "SparklineGroup.HorizontalAxisColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroup-Eigenschaft. Gibt die Farbe der horizontalen Achse in der Sparkline-Gruppe zurück und legt sie fest."
type: docs
url: /de/net/aspose.cells.charts/sparklinegroup/horizontalaxiscolor/
---
## SparklineGroup.HorizontalAxisColor property

Liest und legt die Farbe der horizontalen Achse in der Sparkline-Gruppe fest.

```csharp
public CellsColor HorizontalAxisColor { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyHorizontalAxisColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(3);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(4);

            // Sparkline-Gruppe erstellen
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 3;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A4", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Farbe der horizontalen Achse festlegen
            CellsColor axisColor = workbook.CreateCellsColor();
            axisColor.Color = Color.Blue;
            group.HorizontalAxisColor = axisColor;
            group.ShowHorizontalAxis = true;

            // Speichere die Arbeitsmappe
            workbook.Save("SparklineHorizontalAxisColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


