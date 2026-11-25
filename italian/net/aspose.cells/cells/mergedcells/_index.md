---
title: "Cells.MergedCells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Ottiene la collezione di celle unite"
type: docs
url: /it/net/aspose.cells/cells/mergedcells/
---
## Cells.MergedCells property

Ottiene la raccolta di celle unite.

```csharp
[Obsolete("Use Cells.GetMergedAreas() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList MergedCells { get; }
```

### Osservazioni

In questa collezione, ogni elemento è una struttura [`CellArea`](../../cellarea/) che rappresenta un'area di celle unite.

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Cells.GetMergedAreas(). Questo metodo sarà rimosso tra 12 mesi a partire da novembre 2023. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsPropertyMergedCellsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Unisci celle in due intervalli diversi
            cells.Merge(0, 0, 2, 2); // Merges A1:B2
            cells.Merge(2, 2, 2, 2); // Merges C3:D4

            // Accedi alla proprietà MergedCells (sola lettura)
            ArrayList mergedRanges = cells.MergedCells;

            // Visualizza il conteggio e gli intervalli iniziali delle celle unite
            Console.WriteLine($"Initial merged cells count: {mergedRanges.Count}");
            foreach (CellArea area in mergedRanges)
            {
                Console.WriteLine($"Merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
            }

            // Dividi il primo intervallo unito
            cells.UnMerge(0, 0, 2, 2);

            // Visualizza il conteggio e gli intervalli aggiornati delle celle unite
            Console.WriteLine($"\nAfter unmerging A1:B2 - Merged cells count: {cells.MergedCells.Count}");
            foreach (CellArea area in cells.MergedCells)
            {
                Console.WriteLine($"Remaining merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
            }

            // Salva il risultato
            workbook.Save("PropertyMergedCellsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


