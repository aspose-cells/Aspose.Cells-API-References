---
title: "Sparkline.Row"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Sparkline-Eigenschaft. Gibt den Zeilenindex der Sparkline zurück"
type: docs
url: /de/net/aspose.cells.charts/sparkline/row/
---
## Sparkline.Row property

Gibt den Zeilenindex des Sparkline zurück.

```csharp
public int Row { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyRowDemo
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
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 0,
                StartColumn = 4,
                EndColumn = 4
            };

            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];

            // Sparkline bei Zeile 0, Spalte 4 hinzufügen
            int sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
            Sparkline sparkline = group.Sparklines[sparklineIndex];

            // Zeilenposition anzeigen (schreibgeschützte Eigenschaft)
            Console.WriteLine("Sparkline row position: " + sparkline.Row);

            // Um die Position zu ändern, müssen wir die Sparkline entfernen und neu erstellen
            group.Sparklines.RemoveAt(sparklineIndex);
            sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 2, 4); // New position at row 2
            sparkline = group.Sparklines[sparklineIndex];
            Console.WriteLine("New sparkline row position: " + sparkline.Row);

            // Arbeitsmappe speichern.
            workbook.Save("SparklineRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


