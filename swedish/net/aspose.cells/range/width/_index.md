---
title: "Range.Width"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-egenskap. Hämtar bredden på ett range i punkter"
type: docs
url: /sv/net/aspose.cells/range/width/
---
## Range.Width property

Hämtar bredden på ett område i punkter.

```csharp
public double Width { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in kolumnbredder för att demonstrera Width-egenskapen
            worksheet.Cells.SetColumnWidth(1, 20); // Column B width = 20
            worksheet.Cells.SetColumnWidth(2, 30); // Column C width = 30
            
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Visa range-bredd (summan av kolumnbredder i range)
            Console.WriteLine("Range Width: " + range.Width);
            
            // Visa individuella egenskaper för verifiering
            Console.WriteLine("Range Left Position: " + range.Left);
            Console.WriteLine("Range Top Position: " + range.Top);
            Console.WriteLine("Range Height: " + range.Height);
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


