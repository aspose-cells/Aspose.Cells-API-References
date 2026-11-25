---
title: "Range.RowCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Restituisce il numero di righe nell'intervallo"
type: docs
url: /it/net/aspose.cells/range/rowcount/
---
## Range.RowCount property

Ottiene il conteggio delle righe nell'intervallo.

```csharp
public int RowCount { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRowCountDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea dati di esempio nelle celle A1:B10
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 2; col++)
                {
                    worksheet.Cells[row, col].Value = $"Row{row + 1}Col{col + 1}";
                }
            }

            // Crea un intervallo denominato che copre A1:B10
            worksheet.Cells.CreateRange("A1", "B10").Name = "testRange";
            
            // Ottieni l'intervallo denominato
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("testRange");
            
            // Dimostra la proprietà RowCount
            Console.WriteLine($"Range starts at row: {range.FirstRow}");
            Console.WriteLine($"Range row count: {range.RowCount}");
            Console.WriteLine($"Range starts at column: {range.FirstColumn}");
            Console.WriteLine($"Range column count: {range.ColumnCount}");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


