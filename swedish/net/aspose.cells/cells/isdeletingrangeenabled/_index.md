---
title: "Cells.IsDeletingRangeEnabled"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Kontrollera om intervallet kan raderas"
type: docs
url: /sv/net/aspose.cells/cells/isdeletingrangeenabled/
---
## Cells.IsDeletingRangeEnabled method

Kontrollera om området kan tas bort.

```csharp
public bool IsDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startradindex för intervallet. |
| startColumn | Int32 | Startkolumnindex för intervallet. |
| totalRows | Int32 | Antalet rader i intervallet. |
| totalColumns | Int32 | Antalet kolumner i intervallet. |

### Exempel

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

            // Fyll i exempeldata i cellerna A1:C5
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    cells[row, col].Value = $"Data{row}_{col}";
                }
            }

            try
            {
                // Kontrollera om radering av 5 rader x 3 kolumner från A1 är aktiverad
                bool canDelete = cells.IsDeletingRangeEnabled(0, 0, 5, 3);
                Console.WriteLine($"Can delete range: {canDelete}");

                if (canDelete)
                {
                    // Radera intervallet A1:C5 och flytta cellerna uppåt
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

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


