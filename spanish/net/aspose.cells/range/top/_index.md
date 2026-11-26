---
title: "Range.Top"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Obtiene la distancia en puntos desde el borde superior de la fila 1 hasta el borde superior del rango."
type: docs
url: /es/net/aspose.cells/range/top/
---
## Range.Top property

Obtiene la distancia, en puntos, desde el borde superior de la fila 1 hasta el borde superior del rango.

```csharp
public double Top { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyTopDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un rango y establecer algunos valores.
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            range[0, 0].PutValue("Test");
            
            // Demostrar el uso de la propiedad Top.
            Console.WriteLine("Range Top position: " + range.Top);
            Console.WriteLine("Range Height: " + range.Height);
            Console.WriteLine("Range Left position: " + range.Left);
            Console.WriteLine("Range Width: " + range.Width);
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


