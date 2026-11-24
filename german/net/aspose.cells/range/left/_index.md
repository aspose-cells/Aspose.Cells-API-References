---
title: "Range.Left"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Eigenschaft. Gibt den Abstand in Punkten von der linken Kante der Spalte A bis zur linken Kante des Bereichs zurück"
type: docs
url: /de/net/aspose.cells/range/left/
---
## Range.Left property

Liefert den Abstand in Punkten von der linken Kante der Spalte A zur linken Kante des Bereichs.

```csharp
public double Left { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyLeftDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen Bereich von B2 bis C4
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Demonstriere die Verwendung der Left-Eigenschaft
            Console.WriteLine("Range Left position: " + range.Left);
            Console.WriteLine("Range Width: " + range.Width);
            
            // Berechne erwartete Werte basierend auf dem Testfall
            double expectedLeft = 64 / 96.0 * 72;
            Console.WriteLine("Expected Left position: " + expectedLeft);
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


