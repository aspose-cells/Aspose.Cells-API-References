---
title: "Cell.IsMerged"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Prüft, ob eine Zelle Teil eines zusammengeführten Bereichs ist oder nicht"
type: docs
url: /de/net/aspose.cells/cell/ismerged/
---
## Cell.IsMerged property

Überprüft, ob eine Zelle Teil eines zusammengeführten Bereichs ist oder nicht.

```csharp
public bool IsMerged { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsMergedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zellen A1 bis B2 zusammenführen
            worksheet.Cells.Merge(0, 0, 2, 2);

            // Überprüfen Sie, ob Zelle A1 zusammengeführt ist
            bool isMerged = worksheet.Cells["A1"].IsMerged;
            Console.WriteLine("Is cell A1 merged? " + isMerged);

            // Überprüfen Sie, ob Zelle C1 zusammengeführt ist (sollte false sein)
            isMerged = worksheet.Cells["C1"].IsMerged;
            Console.WriteLine("Is cell C1 merged? " + isMerged);

            // Speichere die Arbeitsmappe
            workbook.Save("MergedCellsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


