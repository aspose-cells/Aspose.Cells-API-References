---
title: "Worksheet.CellWatches"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt die Sammlung von Zellen in diesem Arbeitsblatt zurück, die im Überwachungsfenster beobachtet werden"
type: docs
url: /de/net/aspose.cells/worksheet/cellwatches/
---
## Worksheet.CellWatches property

Liest die Sammlung von Zellen dieses Arbeitsblatts, die im 'Watch Window' überwacht werden.

```csharp
public CellWatchCollection CellWatches { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCellWatchesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zelle B2 hinzu
            sheet.Cells["B2"].PutValue("Sample Data");

            // Füge Zellüberwachung für B2 hinzu
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Zeige Überwachungsinformationen an
            Console.WriteLine($"Cell Watch Added - Index: {watchIndex}");
            Console.WriteLine($"Cell Name: {cellWatch.CellName}");
            Console.WriteLine($"Row: {cellWatch.Row}, Column: {cellWatch.Column}");

            // Speichere die Arbeitsmappe
            workbook.Save("CellWatchDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellWatchCollection](../../cellwatchcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


