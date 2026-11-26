---
title: "Range.Intersect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Devuelve un objeto Range que representa la intersección rectangular de dos rangos"
type: docs
url: /es/net/aspose.cells/range/intersect/
---
## Range.Intersect method

Devuelve un objeto [`Range`](../) que representa la intersección rectangular de dos rangos.

```csharp
public Range Intersect(Range range)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rango | Rango | El rango intersectado. |

### Valor de retorno

Devuelve un objeto [`Range`](../)

### Observaciones

Si los dos rangos no se intersectan, devuelve null.

### Ejemplos

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

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


