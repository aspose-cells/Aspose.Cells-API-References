---
title: "Range.Top"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-egenskap. Hämtar avståndet i punkter från den övre kanten av rad 1 till den övre kanten av området"
type: docs
url: /sv/net/aspose.cells/range/top/
---
## Range.Top property

Hämtar avståndet, i punkter, från överkanten av rad 1 till överkanten av området.

```csharp
public double Top { get; }
```

### Exempel

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
            
            // Skapa ett område och ange några värden
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            range[0, 0].PutValue("Test");
            
            // Demonstrera användning av Top-egenskapen
            Console.WriteLine("Range Top position: " + range.Top);
            Console.WriteLine("Range Height: " + range.Height);
            Console.WriteLine("Range Left position: " + range.Left);
            Console.WriteLine("Range Width: " + range.Width);
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


