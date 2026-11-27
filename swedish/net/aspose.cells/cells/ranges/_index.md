---
title: "Cells.Ranges"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar samlingen av Range-objekt som skapas vid körning"
type: docs
url: /sv/net/aspose.cells/cells/ranges/
---
## Cells.Ranges property

Hämtar samlingen av [`Range`](../../range/) objekt som skapas vid körning.

```csharp
public RangeCollection Ranges { get; }
```

### Exempel

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
            
            // Skapa och lägg till ett intervall i Ranges-samlingen
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            
            // Infoga rader och visa att intervallet expanderar
            worksheet.Cells.InsertRows(2, 2, true);
            
            Console.WriteLine($"Range row count after insertion: {cellRange.RowCount}");
        }
    }
}
```

### Se även

* class [RangeCollection](../../rangecollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


