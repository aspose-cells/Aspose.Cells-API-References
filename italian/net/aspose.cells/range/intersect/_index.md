---
title: "Range.Intersect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Restituisce un oggetto Range che rappresenta l'intersezione rettangolare di due intervalli"
type: docs
url: /it/net/aspose.cells/range/intersect/
---
## Range.Intersect method

Restituisce un oggetto [`Range`](../) che rappresenta l'intersezione rettangolare di due intervalli.

```csharp
public Range Intersect(Range range)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | Intervallo | L'intervallo di intersezione. |

### Valore di ritorno

Restituisce un oggetto [`Range`](../)

### Osservazioni

Se i due intervalli non si intersecano, restituisce null.

### Esempi

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

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


