---
title: "Cells.Ranges"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene la collezione di oggetti Range creati a runtime"
type: docs
url: /it/net/aspose.cells/cells/ranges/
---
## Cells.Ranges property

Ottiene la collezione di [`Range`](../../range/) oggetti creati a runtime.

```csharp
public RangeCollection Ranges { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyRangesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea e aggiungi un range alla collezione Ranges
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            
            // Inserisci righe e dimostra che il range si espande
            worksheet.Cells.InsertRows(2, 2, true);
            
            Console.WriteLine($"Range row count after insertion: {cellRange.RowCount}");
        }
    }
}
```

### Vedi anche

* class [RangeCollection](../../rangecollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


