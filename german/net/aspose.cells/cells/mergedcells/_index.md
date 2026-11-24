---
title: "Cells.MergedCells"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Gibt die Sammlung zusammengeführter Zellen zurück"
type: docs
url: /de/net/aspose.cells/cells/mergedcells/
---
## Cells.MergedCells property

Liest die Sammlung zusammengeführter Zellen.

```csharp
[Obsolete("Use Cells.GetMergedAreas() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList MergedCells { get; }
```

### Hinweise

In dieser Sammlung ist jedes Element eine [`CellArea`](../../cellarea/) Struktur, die einen Bereich zusammengeführter Zellen darstellt.

HINWEIS: Diese Methode ist jetzt veraltet. Bitte verwenden Sie stattdessen die Methode Cells.GetMergedAreas(). Diese Methode wird 12 Monate später, seit November 2023, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Zellen in zwei verschiedenen Bereichen zusammenführen
            cells.Merge(0, 0, 2, 2); // Merges A1:B2
            cells.Merge(2, 2, 2, 2); // Merges C3:D4

            // Greifen Sie auf die MergedCells-Eigenschaft zu (schreibgeschützt)
            ArrayList mergedRanges = cells.MergedCells;

            // Anzeigen der anfänglichen Anzahl zusammengeführter Zellen und Bereiche
            Console.WriteLine($"Initial merged cells count: {mergedRanges.Count}");
            foreach (CellArea area in mergedRanges)
            {
                Console.WriteLine($"Merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
            }

            // Den ersten zusammengeführten Bereich aufheben
            cells.UnMerge(0, 0, 2, 2);

            // Anzeigen der aktualisierten Anzahl zusammengeführter Zellen und Bereiche
            Console.WriteLine($"\nAfter unmerging A1:B2 - Merged cells count: {cells.MergedCells.Count}");
            foreach (CellArea area in cells.MergedCells)
            {
                Console.WriteLine($"Remaining merged area: Row[{area.StartRow}-{area.EndRow}], Column[{area.StartColumn}-{area.EndColumn}]");
            }

            // Ergebnis speichern
            workbook.Save("PropertyMergedCellsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


