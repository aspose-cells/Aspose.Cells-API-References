---
title: "Cell.IsMerged"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell‑egenskap. Kontrollerar om en cell är en del av ett sammanslaget område eller inte"
type: docs
url: /sv/net/aspose.cells/cell/ismerged/
---
## Cell.IsMerged property

Kontrollerar om en cell är en del av ett sammanslaget område eller inte.

```csharp
public bool IsMerged { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsMergedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sammanfoga cellerna A1 till B2
            worksheet.Cells.Merge(0, 0, 2, 2);

            // Kontrollera om cell A1 är sammanslagen
            bool isMerged = worksheet.Cells["A1"].IsMerged;
            Console.WriteLine("Is cell A1 merged? " + isMerged);

            // Kontrollera om cell C1 är sammanslagen (ska vara falskt)
            isMerged = worksheet.Cells["C1"].IsMerged;
            Console.WriteLine("Is cell C1 merged? " + isMerged);

            // Spara arbetsboken
            workbook.Save("MergedCellsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


