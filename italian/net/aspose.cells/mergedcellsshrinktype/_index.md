---
title: "Enum MergedCellsShrinkType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.MergedCellsShrinkType enum. Rappresenta la strategia per ridurre le celle unite per operazioni come l'eliminazione di righe/colonne vuote"
type: docs
url: /it/net/aspose.cells/mergedcellsshrinktype/
---
## MergedCellsShrinkType enumeration

Rappresenta la strategia per ridurre le celle unite nelle operazioni come l'eliminazione di righe/colonne vuote.

```csharp
public enum MergedCellsShrinkType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Lascia le celle unite così come sono senza alcuna modifica. |
| ShrinkToFit | `1` | Riduce l'area unita se necessario, rimuovendo le righe dal basso o le colonne da destra, garantendo che tutto il contenuto rimanga visibile. |
| KeepHeaderOnly | `2` | Mantiene solo le righe/colonne di intestazione dell'area unita quando la cella in alto a sinistra dell'area unita non è vuota. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassMergedCellsShrinkTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;

            // Inizializza dati di esempio con celle unite
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            Console.WriteLine("Original worksheet:");
            PrintCellValues(cells);

            // Opzione 1: KeepHeaderOnly
            DeleteBlankOptions opts1 = new DeleteBlankOptions();
            opts1.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankColumns(opts1);
            Console.WriteLine("\nAfter DeleteBlankColumns with KeepHeaderOnly:");
            PrintCellValues(cells);

            // Reimposta foglio di lavoro
            cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            // Opzione 2: Nessuno
            DeleteBlankOptions opts2 = new DeleteBlankOptions();
            opts2.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankColumns(opts2);
            Console.WriteLine("\nAfter DeleteBlankColumns with None:");
            PrintCellValues(cells);

            // Reimposta foglio di lavoro
            cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            // Opzione 3: ShrinkToFit
            DeleteBlankOptions opts3 = new DeleteBlankOptions();
            opts3.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
            cells.DeleteBlankColumns(opts3);
            Console.WriteLine("\nAfter DeleteBlankColumns with ShrinkToFit:");
            PrintCellValues(cells);
        }

        private static void PrintCellValues(Cells cells)
        {
            for (int row = 0; row < 3; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Console.Write($"({row},{col}): {cells[row, col].Value ?? "empty"} | ");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


