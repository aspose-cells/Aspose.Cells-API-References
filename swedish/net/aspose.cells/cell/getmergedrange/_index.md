---
title: "Cell.GetMergedRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Returnerar ett Range-objekt som representerar ett sammanslaget område"
type: docs
url: /sv/net/aspose.cells/cell/getmergedrange/
---
## Cell.GetMergedRange method

Returnerar ett [`Range`](../../range/)-objekt som representerar ett sammanslaget område.

```csharp
public Range GetMergedRange()
```

### Returvärde

[`Range`](../../range/) object. Null if this cell is not merged.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetMergedRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Sammanfoga celler
            cells.Merge(0, 0, 2, 2);

            // Hämta den första cellen
            Cell cell = cells[0, 0];

            // Hämta information om sammanslaget område
            Aspose.Cells.Range mergedRange = cell.GetMergedRange();
            
            // Skriv ut detaljer för sammanslaget område
            Console.WriteLine("Merged Range Details:");
            Console.WriteLine($"First Row: {mergedRange.FirstRow}");
            Console.WriteLine($"First Column: {mergedRange.FirstColumn}");
            Console.WriteLine($"Row Count: {mergedRange.RowCount}");
            Console.WriteLine($"Column Count: {mergedRange.ColumnCount}");
        }
    }
}
```

### Se även

* class [Range](../../range/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


