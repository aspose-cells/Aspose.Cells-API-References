---
title: "UnionRange.RangeCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "UnionRange-Eigenschaft. Gibt die Anzahl der Bereiche zurück"
type: docs
url: /de/net/aspose.cells/unionrange/rangecount/
---
## UnionRange.RangeCount property

Ermittelt die Anzahl der Bereiche.

```csharp
public int RangeCount { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyRangeCountDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            Aspose.Cells.Range r1 = cells.CreateRange("B1:C10");
            Aspose.Cells.Range r2 = cells.CreateRange("C2:D10");
            
            UnionRange unionRange = r1.UnionRanges(new Aspose.Cells.Range[] { r2 });
            
            Console.WriteLine("RangeCount: " + unionRange.RangeCount);
            for (int i = 0; i < unionRange.RangeCount; i++)
            {
                Console.WriteLine($"Range {i+1} Address: {unionRange.Ranges[i].Address}");
            }
        }
    }
}
```

### Siehe auch

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


