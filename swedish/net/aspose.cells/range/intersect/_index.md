---
title: "Range.Intersect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range‑metod. Returnerar ett Range‑objekt som representerar den rektangulära skärningen av två områden"
type: docs
url: /sv/net/aspose.cells/range/intersect/
---
## Range.Intersect method

Returnerar ett [`Range`](../)‑objekt som representerar den rektangulära skärningen av två områden.

```csharp
public Range Intersect(Range range)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | Range | Det skärande området. |

### Returvärde

Returnerar ett [`Range`](../)‑objekt

### Anmärkningar

Om de två områdena inte skär varandra, returneras null.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodIntersectWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            Aspose.Cells.Range range1 = cells.CreateRange("A1:A5");
            Aspose.Cells.Range range2 = cells.CreateRange("A3:A10");
            
            Aspose.Cells.Range intersectRange = range1.Intersect(range2);
            
            Console.WriteLine("Intersected range: " + intersectRange.Address);
            workbook.Save("IntersectDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


