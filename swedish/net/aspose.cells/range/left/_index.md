---
title: "Range.Left"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range‑egenskap. Hämtar avståndet i punkter från vänstra kanten av kolumn A till vänstra kanten av området"
type: docs
url: /sv/net/aspose.cells/range/left/
---
## Range.Left property

Hämtar avståndet, i punkter, från vänstra kanten av kolumn A till vänstra kanten av området.

```csharp
public double Left { get; }
```

### Exempel

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
            
            // Skapa ett område från B2 till C4
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Demonstrera användning av Left‑egenskapen
            Console.WriteLine("Range Left position: " + range.Left);
            Console.WriteLine("Range Width: " + range.Width);
            
            // Beräkna förväntade värden baserat på testfallet
            double expectedLeft = 64 / 96.0 * 72;
            Console.WriteLine("Expected Left position: " + expectedLeft);
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


