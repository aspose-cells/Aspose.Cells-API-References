---
title: "SparklineGroup.ResetRanges"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroup-Methode. Setzt den Datenbereich und den Positionsbereich der Sparkline-Gruppe zurück. Diese Methode löscht die ursprünglichen Sparkline-Elemente in der Gruppe und erstellt neue Sparkline-Elemente für die neuen Bereiche."
type: docs
url: /de/net/aspose.cells.charts/sparklinegroup/resetranges/
---
## SparklineGroup.ResetRanges method

Setzt den Datenbereich und den Positionsbereich der Sparkline-Gruppe zurück. Diese Methode löscht die ursprünglichen Sparkline-Elemente in der Gruppe und erstellt neue Sparkline-Elemente für die neuen Bereiche.

```csharp
public void ResetRanges(string dataRange, bool isVertical, CellArea locationRange)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataRange | String | Gibt den neuen Datenbereich der Sparkline-Gruppe an. |
| isVertical | Boolean | Gibt an, ob die Sparklines aus dem neuen Datenbereich zeilenweise oder spaltenweise dargestellt werden sollen. |
| locationRange | CellArea | Gibt an, wo die Sparklines platziert werden sollen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupMethodResetRangesWithStringBooleanCellAreaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Definiert den CellArea für die Sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Fügt der Arbeitsmappe eine Sparkline-Gruppe hinzu
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);

            SparklineGroup group = sheet.SparklineGroups[idx];

            // Parameter für ResetRanges vorbereiten
            string dataRange = "A1:D1";
            bool isVertical = false;
            CellArea locationRange = CellArea.CreateCellArea(6, 5, 6, 5);

            try
            {
                // Rufen Sie ResetRanges mit den Parametern (String, Boolean, CellArea) auf
                group.ResetRanges(dataRange, isVertical, locationRange);

                Console.WriteLine("ResetRanges method executed successfully with parameters (String, Boolean, CellArea)");
                
                
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetRanges method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("SparklineGroupResetRangesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


