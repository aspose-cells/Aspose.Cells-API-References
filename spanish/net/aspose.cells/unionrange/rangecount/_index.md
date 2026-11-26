---
title: "UnionRange.RangeCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad UnionRange. Obtiene el recuento de los rangos"
type: docs
url: /es/net/aspose.cells/unionrange/rangecount/
---
## UnionRange.RangeCount property

Obtiene la cantidad de los rangos.

```csharp
public int RangeCount { get; }
```

### Ejemplos

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

### Ver también

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


