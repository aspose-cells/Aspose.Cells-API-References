---
title: "Enum MergedCellsShrinkType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.MergedCellsShrinkType enum. Repräsentiert die Strategie zum Verkleinern zusammengeführter Zellen für Vorgänge wie das Löschen leerer Zeilen/Spalten."
type: docs
url: /de/net/aspose.cells/mergedcellsshrinktype/
---
## MergedCellsShrinkType enumeration

Stellt die Strategie zum Verkleinern zusammengeführter Zellen für Vorgänge wie das Löschen leerer Zeilen/Spalten dar.

```csharp
public enum MergedCellsShrinkType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Lässt die zusammengeführten Zellen unverändert. |
| ShrinkToFit | `1` | Verkleinert den zusammengeführten Bereich bei Bedarf, indem Zeilen von unten oder Spalten von rechts entfernt werden, wobei sichergestellt wird, dass alle Inhalte sichtbar bleiben. |
| KeepHeaderOnly | `2` | Behält nur die Kopfzeilen/Spalten des zusammengeführten Bereichs, wenn die obere linke Zelle des zusammengeführten Bereichs nicht leer ist. |

### Beispiele

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

            // Beispieldaten mit zusammengeführten Zellen initialisieren
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            Console.WriteLine("Original worksheet:");
            PrintCellValues(cells);

            // Option 1: NurKopfzeileBehalten
            DeleteBlankOptions opts1 = new DeleteBlankOptions();
            opts1.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankColumns(opts1);
            Console.WriteLine("\nAfter DeleteBlankColumns with KeepHeaderOnly:");
            PrintCellValues(cells);

            // Arbeitsblatt zurücksetzen
            cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            // Option 2: Keine
            DeleteBlankOptions opts2 = new DeleteBlankOptions();
            opts2.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankColumns(opts2);
            Console.WriteLine("\nAfter DeleteBlankColumns with None:");
            PrintCellValues(cells);

            // Arbeitsblatt zurücksetzen
            cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            // Option 3: VerkleinernUmAnpassen
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

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


