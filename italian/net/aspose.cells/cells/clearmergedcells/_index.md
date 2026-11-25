---
title: "Cells.ClearMergedCells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Cancella tutti gli intervalli uniti"
type: docs
url: /it/net/aspose.cells/cells/clearmergedcells/
---
## Cells.ClearMergedCells method

Cancella tutti i range uniti.

```csharp
public void ClearMergedCells()
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearMergedCellsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea celle unite in A1:B2
            worksheet.Cells.Merge(0, 0, 2, 2);
            Console.WriteLine($"Merged areas before clearing: {worksheet.Cells.GetMergedAreas().Length}");

            try
            {
                // Cancella tutte le celle unite nel foglio di lavoro
                worksheet.Cells.ClearMergedCells();
                Console.WriteLine("Method executed successfully");
                Console.WriteLine($"Merged areas after clearing: {worksheet.Cells.GetMergedAreas().Length}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearMergedCells method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("ClearMergedCellsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


