---
title: "Range.Intersect"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Gibt ein Range-Objekt zurück, das die rechteckige Schnittmenge zweier Bereiche darstellt"
type: docs
url: /de/net/aspose.cells/range/intersect/
---
## Range.Intersect method

Gibt ein [`Range`](../)-Objekt zurück, das die rechteckige Schnittmenge zweier Bereiche darstellt.

```csharp
public Range Intersect(Range range)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | Range | Der sich überschneidende Bereich. |

### Rückgabewert

Gibt ein [`Range`](../)-Objekt zurück

### Hinweise

Wenn die beiden Bereiche nicht überschneiden, wird null zurückgegeben.

### Beispiele

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

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


