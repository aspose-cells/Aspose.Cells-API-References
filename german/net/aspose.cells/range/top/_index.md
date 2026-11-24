---
title: "Range.Top"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Gibt den Abstand in Punkten von der oberen Kante von Zeile 1 bis zur oberen Kante des Bereichs zurück"
type: docs
url: /de/net/aspose.cells/range/top/
---
## Range.Top property

Liefert den Abstand in Punkten von der oberen Kante der Zeile 1 zur oberen Kante des Bereichs.

```csharp
public double Top { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyTopDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen Bereich und setze einige Werte
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            range[0, 0].PutValue("Test");
            
            // Demonstriere die Verwendung der Top‑Eigenschaft
            Console.WriteLine("Range Top position: " + range.Top);
            Console.WriteLine("Range Height: " + range.Height);
            Console.WriteLine("Range Left position: " + range.Left);
            Console.WriteLine("Range Width: " + range.Width);
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


