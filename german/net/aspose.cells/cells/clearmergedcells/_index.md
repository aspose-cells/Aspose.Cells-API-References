---
title: "Cells.ClearMergedCells"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Löscht alle zusammengeführten Bereiche"
type: docs
url: /de/net/aspose.cells/cells/clearmergedcells/
---
## Cells.ClearMergedCells method

Löscht alle zusammengeführten Bereiche.

```csharp
public void ClearMergedCells()
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearMergedCellsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle zusammengeführte Zellen in A1:B2
            worksheet.Cells.Merge(0, 0, 2, 2);
            Console.WriteLine($"Merged areas before clearing: {worksheet.Cells.GetMergedAreas().Length}");

            try
            {
                // Alle zusammengeführten Zellen im Arbeitsblatt löschen
                worksheet.Cells.ClearMergedCells();
                Console.WriteLine("Method executed successfully");
                Console.WriteLine($"Merged areas after clearing: {worksheet.Cells.GetMergedAreas().Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearMergedCells method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("ClearMergedCellsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


