---
title: "Cells.Ranges"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Gibt die Sammlung von Range-Objekten zurück, die zur Laufzeit erstellt wurden"
type: docs
url: /de/net/aspose.cells/cells/ranges/
---
## Cells.Ranges property

Gibt die Sammlung von [`Range`](../../range/) Objekten zurück, die zur Laufzeit erstellt wurden.

```csharp
public RangeCollection Ranges { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyRangesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstellen und einen Bereich zur Ranges-Sammlung hinzufügen
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            
            // Zeilen einfügen und demonstrieren, dass der Bereich erweitert wird
            worksheet.Cells.InsertRows(2, 2, true);
            
            Console.WriteLine($"Range row count after insertion: {cellRange.RowCount}");
        }
    }
}
```

### Siehe auch

* class [RangeCollection](../../rangecollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


