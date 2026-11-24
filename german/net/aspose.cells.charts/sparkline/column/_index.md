---
title: "Sparkline.Column"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Sparkline-Eigenschaft. Gibt den Spaltenindex der Sparkline zurück"
type: docs
url: /de/net/aspose.cells.charts/sparkline/column/
---
## Sparkline.Column property

Gibt den Spaltenindex des Sparkline zurück.

```csharp
public int Column { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyColumnDemo
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
            
            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];

            // Fügen Sie eine Sparkline in Spalte 4 ein und demonstrieren Sie die Column-Eigenschaft
            int sparklineIndex = group.Sparklines.Add("A1:D1", 0, 4);
            Sparkline sparkline = group.Sparklines[sparklineIndex];

            // Spalten-Eigenschaft (nur lesbar) anzeigen
            Console.WriteLine("Sparkline Column: " + sparkline.Column);

            // Um die Spaltenposition zu ändern, müssen wir die Sparkline entfernen und erneut hinzufügen
            group.Sparklines.RemoveAt(sparklineIndex);
            sparklineIndex = group.Sparklines.Add("A1:D1", 0, 5); // New column position
            sparkline = group.Sparklines[sparklineIndex];
            Console.WriteLine("New Sparkline Column: " + sparkline.Column);

            // Arbeitsmappe speichern.
            workbook.Save("SparklineColumnDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


