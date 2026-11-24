---
title: "Range.RowCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Gibt die Anzahl der Zeilen im Bereich zurück"
type: docs
url: /de/net/aspose.cells/range/rowcount/
---
## Range.RowCount property

Liefert die Anzahl der Zeilen im Bereich.

```csharp
public int RowCount { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRowCountDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle Beispieldaten in den Zellen A1:B10
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 2; col++)
                {
                    worksheet.Cells[row, col].Value = $"Row{row + 1}Col{col + 1}";
                }
            }

            // Erstelle einen benannten Bereich, der A1:B10 abdeckt
            worksheet.Cells.CreateRange("A1", "B10").Name = "testRange";
            
            // Hole den benannten Bereich
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("testRange");
            
            // Demonstriere die RowCount-Eigenschaft
            Console.WriteLine($"Range starts at row: {range.FirstRow}");
            Console.WriteLine($"Range row count: {range.RowCount}");
            Console.WriteLine($"Range starts at column: {range.FirstColumn}");
            Console.WriteLine($"Range column count: {range.ColumnCount}");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


