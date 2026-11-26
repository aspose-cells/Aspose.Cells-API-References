---
title: "Range.Height"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Obtiene el ancho de un rango en puntos"
type: docs
url: /es/net/aspose.cells/range/height/
---
## Range.Height property

Obtiene el ancho de un rango en puntos.

```csharp
public double Height { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer alturas de fila para la demostración
            worksheet.Cells.SetRowHeight(1, 15.0); // Row 2 (0-based index 1)
            worksheet.Cells.SetRowHeight(2, 20.0); // Row 3
            worksheet.Cells.SetRowHeight(3, 25.0); // Row 4

            // Crear un rango que abarque las filas 2-4 (B2:C4)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // Demostrar la propiedad Height
            Console.WriteLine("Range Height: " + range.Height);
            Console.WriteLine("Calculated Height (sum of row heights): " + 
                (worksheet.Cells.GetRowHeight(1) + 
                 worksheet.Cells.GetRowHeight(2) + 
                 worksheet.Cells.GetRowHeight(3)));
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


