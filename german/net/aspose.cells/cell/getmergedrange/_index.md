---
title: "Cell.GetMergedRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt ein Range-Objekt zurück, das einen zusammengeführten Bereich darstellt"
type: docs
url: /de/net/aspose.cells/cell/getmergedrange/
---
## Cell.GetMergedRange method

Gibt ein [`Range`](../../range/)‑Objekt zurück, das einen zusammengeführten Bereich darstellt.

```csharp
public Range GetMergedRange()
```

### Rückgabewert

[`Range`](../../range/) object. Null if this cell is not merged.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetMergedRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Zellen zusammenführen
            cells.Merge(0, 0, 2, 2);

            // Hole die erste Zelle
            Cell cell = cells[0, 0];

            // Informationen zum zusammengeführten Bereich abrufen
            Aspose.Cells.Range mergedRange = cell.GetMergedRange();
            
            // Details des zusammengeführten Bereichs ausgeben
            Console.WriteLine("Merged Range Details:");
            Console.WriteLine($"First Row: {mergedRange.FirstRow}");
            Console.WriteLine($"First Column: {mergedRange.FirstColumn}");
            Console.WriteLine($"Row Count: {mergedRange.RowCount}");
            Console.WriteLine($"Column Count: {mergedRange.ColumnCount}");
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


