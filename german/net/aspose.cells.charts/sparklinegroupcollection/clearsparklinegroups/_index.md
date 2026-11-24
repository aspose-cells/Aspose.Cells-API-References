---
title: "SparklineGroupCollection.ClearSparklineGroups"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SparklineGroupCollection-Methode. Löscht die Sparkline-Gruppen, die einen Zellbereich überlappen."
type: docs
url: /de/net/aspose.cells.charts/sparklinegroupcollection/clearsparklinegroups/
---
## SparklineGroupCollection.ClearSparklineGroups method

Löscht die Sparkline-Gruppen, die einen Zellbereich überlappen.

```csharp
public void ClearSparklineGroups(CellArea cellArea)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellArea | CellArea | Gibt den Zellbereich an |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodClearSparklineGroupsWithCellAreaDemo
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


            try
            {
                // Rufen Sie die ClearSparklineGroups-Methode mit dem CellArea-Parameter auf
                sheet.SparklineGroups.ClearSparklineGroups(ca);
                
                Console.WriteLine("Sparkline groups cleared successfully for the specified cell area.");
                
                // Überprüfen Sie die Anzahl der Sparkline-Gruppen nach dem Löschen
                Console.WriteLine($"Remaining sparkline groups count: {sheet.SparklineGroups.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearSparklineGroups method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("ClearSparklineGroupsWithCellAreaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


