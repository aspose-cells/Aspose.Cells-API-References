---
title: "CellWatch.Row"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellWatch-Eigenschaft. Liest und schreibt die Zeile der Zelle."
type: docs
url: /de/net/aspose.cells/cellwatch/row/
---
## CellWatch.Row property

Ermittelt und setzt die Zeile der Zelle.

```csharp
public int Row { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zelle B2 hinzu
            sheet.Cells["B2"].PutValue("Sample Data");

            // Füge CellWatch für B2 hinzu.
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Demonstriere die Row-Eigenschaft.
            Console.WriteLine($"Original Row: {cellWatch.Row}");
            cellWatch.Row = 1; // Set row to 1 (0-based) for B2
            Console.WriteLine($"Updated Row: {cellWatch.Row}");

            // Überprüfe die Zellreferenz.
            Console.WriteLine($"Cell Reference: {sheet.Cells[cellWatch.Row, cellWatch.Column].Name}");

            workbook.Save("CellWatchRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


