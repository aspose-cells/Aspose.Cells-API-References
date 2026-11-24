---
title: "Cells.CountLarge"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Gibt die Gesamtzahl der instanziierten Cell-Objekte zurück"
type: docs
url: /de/net/aspose.cells/cells/countlarge/
---
## Cells.CountLarge property

Ruft die Gesamtanzahl der instanziierten Cell‑Objekte ab.

```csharp
public long CountLarge { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyCountLargeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Daten zu den Zellen hinzufügen
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B2"].PutValue("World");
            worksheet.Cells["C3"].PutValue(123);
            
            // Demonstration der CountLarge-Eigenschaft
            long cellCount = worksheet.Cells.CountLarge;
            Console.WriteLine($"Total cells in worksheet: {cellCount}");
            
            // Papiergröße zur Demonstration anzeigen
            Console.WriteLine($"Paper Height: {worksheet.PageSetup.PaperHeight}");
            Console.WriteLine($"Paper Width: {worksheet.PageSetup.PaperWidth}");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


