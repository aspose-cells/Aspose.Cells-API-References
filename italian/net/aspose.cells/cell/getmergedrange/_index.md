---
title: "Cell.GetMergedRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Restituisce un oggetto Range che rappresenta un intervallo unito"
type: docs
url: /it/net/aspose.cells/cell/getmergedrange/
---
## Cell.GetMergedRange method

Restituisce un oggetto [`Range`](../../range/) che rappresenta un intervallo unito.

```csharp
public Range GetMergedRange()
```

### Valore di ritorno

[`Range`](../../range/) object. Null if this cell is not merged.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetMergedRangeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Unisci le celle
            cells.Merge(0, 0, 2, 2);

            // Ottieni la prima cella
            Cell cell = cells[0, 0];

            // Ottieni le informazioni dell'intervallo unito
            Aspose.Cells.Range mergedRange = cell.GetMergedRange();
            
            // Emetti i dettagli dell'intervallo unito
            Console.WriteLine("Merged Range Details:");
            Console.WriteLine($"First Row: {mergedRange.FirstRow}");
            Console.WriteLine($"First Column: {mergedRange.FirstColumn}");
            Console.WriteLine($"Row Count: {mergedRange.RowCount}");
            Console.WriteLine($"Column Count: {mergedRange.ColumnCount}");
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


