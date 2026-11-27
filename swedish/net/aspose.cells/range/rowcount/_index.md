---
title: "Range.RowCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-egenskap. Hämtar antalet rader i området"
type: docs
url: /sv/net/aspose.cells/range/rowcount/
---
## Range.RowCount property

Hämtar antalet rader i området.

```csharp
public int RowCount { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRowCountDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa exempeldata i cellerna A1:B10
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 2; col++)
                {
                    worksheet.Cells[row, col].Value = $"Row{row + 1}Col{col + 1}";
                }
            }

            // Skapa ett namngivet område som täcker A1:B10
            worksheet.Cells.CreateRange("A1", "B10").Name = "testRange";
            
            // Hämta det namngivna området
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("testRange");
            
            // Demonstrera RowCount-egenskapen
            Console.WriteLine($"Range starts at row: {range.FirstRow}");
            Console.WriteLine($"Range row count: {range.RowCount}");
            Console.WriteLine($"Range starts at column: {range.FirstColumn}");
            Console.WriteLine($"Range column count: {range.ColumnCount}");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


