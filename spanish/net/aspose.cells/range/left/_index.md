---
title: "Range.Left"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Obtiene la distancia en puntos desde el borde izquierdo de la columna A hasta el borde izquierdo del rango"
type: docs
url: /es/net/aspose.cells/range/left/
---
## Range.Left property

Obtiene la distancia, en puntos, desde el borde izquierdo de la columna A hasta el borde izquierdo del rango.

```csharp
public double Left { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyLeftDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un rango de B2 a C4
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Demostrar el uso de la propiedad Left
            Console.WriteLine("Range Left position: " + range.Left);
            Console.WriteLine("Range Width: " + range.Width);
            
            // Calcular los valores esperados basados en el caso de prueba
            double expectedLeft = 64 / 96.0 * 72;
            Console.WriteLine("Expected Left position: " + expectedLeft);
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


