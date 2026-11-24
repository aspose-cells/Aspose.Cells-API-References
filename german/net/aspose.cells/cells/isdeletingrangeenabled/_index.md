---
title: "Cells.IsDeletingRangeEnabled"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Prüfe, ob der Bereich gelöscht werden kann"
type: docs
url: /de/net/aspose.cells/cells/isdeletingrangeenabled/
---
## Cells.IsDeletingRangeEnabled method

Überprüfen, ob der Bereich gelöscht werden kann.

```csharp
public bool IsDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Der Startzeilenindex des Bereichs. |
| startColumn | Int32 | Der Startspaltenindex des Bereichs. |
| totalRows | Int32 | Die Anzahl der Zeilen im Bereich. |
| totalColumns | Int32 | Die Anzahl der Spalten im Bereich. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodIsDeletingRangeEnabledWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispieldaten in den Zellen A1:C5 einfügen
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    cells[row, col].Value = $"Data{row}_{col}";
                }
            }

            try
            {
                // Prüfe, ob das Löschen von 5 Zeilen x 3 Spalten ab A1 aktiviert ist
                bool canDelete = cells.IsDeletingRangeEnabled(0, 0, 5, 3);
                Console.WriteLine($"Can delete range: {canDelete}");

                if (canDelete)
                {
                    // Lösche den Bereich A1:C5 und verschiebe die Zellen nach oben
                    cells.DeleteRange(0, 0, 4, 2, ShiftType.Up);
                    Console.WriteLine("Deleted range A1:C5 successfully");
                }

                workbook.Save("IsDeletingRangeEnabledOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during range deletion: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


