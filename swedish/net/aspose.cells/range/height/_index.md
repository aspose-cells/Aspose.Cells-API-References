---
title: "Range.Height"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-egenskap. Hämtar bredden på ett range i punkter"
type: docs
url: /sv/net/aspose.cells/range/height/
---
## Range.Height property

Hämtar bredden på ett område i punkter.

```csharp
public double Height { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in radhöjder för demonstration
            worksheet.Cells.SetRowHeight(1, 15.0); // Row 2 (0-based index 1)
            worksheet.Cells.SetRowHeight(2, 20.0); // Row 3
            worksheet.Cells.SetRowHeight(3, 25.0); // Row 4

            // Skapa ett område som sträcker sig över raderna 2-4 (B2:C4)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Demonstrera Height-egenskapen
            Console.WriteLine("Range Height: " + range.Height);
            Console.WriteLine("Calculated Height (sum of row heights): " + 
                (worksheet.Cells.GetRowHeight(1) + 
                 worksheet.Cells.GetRowHeight(2) + 
                 worksheet.Cells.GetRowHeight(3)));
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


