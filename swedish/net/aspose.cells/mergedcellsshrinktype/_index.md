---
title: "Enum MergedCellsShrinkType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.MergedCellsShrinkType enum. Representerar strategin för att krympa sammanslagna celler för operationer såsom att ta bort tomma rader/kolumner"
type: docs
url: /sv/net/aspose.cells/mergedcellsshrinktype/
---
## MergedCellsShrinkType enumeration

Representerar strategin för att krympa sammanslagna celler för operationer som att ta bort tomma rader/kolumner.

```csharp
public enum MergedCellsShrinkType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Lämnar de sammanslagna cellerna som de är utan någon ändring. |
| ShrinkToFit | `1` | Krymper det sammanslagna området vid behov genom att ta bort rader från botten eller kolumner från höger, samtidigt som allt innehåll förblir synligt. |
| KeepHeaderOnly | `2` | Behåller endast rubrikraderna/kolumnerna i det sammanslagna området när den övre vänstra cellen i området inte är tom. |

### Exempel

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

            // Initiera exempeldata med sammanslagna celler
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            Console.WriteLine("Original worksheet:");
            PrintCellValues(cells);

            // Alternativ 1: KeepHeaderOnly
            DeleteBlankOptions opts1 = new DeleteBlankOptions();
            opts1.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankColumns(opts1);
            Console.WriteLine("\nAfter DeleteBlankColumns with KeepHeaderOnly:");
            PrintCellValues(cells);

            // Återställ kalkylbladet
            cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            // Alternativ 2: None
            DeleteBlankOptions opts2 = new DeleteBlankOptions();
            opts2.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankColumns(opts2);
            Console.WriteLine("\nAfter DeleteBlankColumns with None:");
            PrintCellValues(cells);

            // Återställ kalkylbladet
            cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            // Alternativ 3: ShrinkToFit
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

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


