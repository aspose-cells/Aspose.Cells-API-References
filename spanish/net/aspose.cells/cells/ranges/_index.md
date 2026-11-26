---
title: "Cells.Ranges"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene la colección de objetos Range creados en tiempo de ejecución"
type: docs
url: /es/net/aspose.cells/cells/ranges/
---
## Cells.Ranges property

Obtiene la colección de objetos [`Range`](../../range/) creados en tiempo de ejecución.

```csharp
public RangeCollection Ranges { get; }
```

### Ejemplos

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
            
            // Crea y añade un rango a la colección Ranges
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            
            // Inserta filas y demuestra que el rango se expande
            worksheet.Cells.InsertRows(2, 2, true);
            
            Console.WriteLine($"Range row count after insertion: {cellRange.RowCount}");
        }
    }
}
```

### Ver también

* class [RangeCollection](../../rangecollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


