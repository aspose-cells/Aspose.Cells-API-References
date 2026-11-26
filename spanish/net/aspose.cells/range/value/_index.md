---
title: "Range.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Range. Obtiene y establece el valor del rango."
type: docs
url: /es/net/aspose.cells/range/value/
---
## Range.Value property

Obtiene y establece el valor del rango.

```csharp
public object Value { get; set; }
```

### Observaciones

Si el rango contiene múltiples celdas, el objeto devuelto/aplicado debe ser un objeto Array bidimensional.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un rango que comience en A1 cubriendo 3x3 celdas.
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");

            // Establecer una matriz 2D como valor del rango.
            int[,] values = new int[3, 3] { { 1, 2, 3 }, { 4, 5, 6 }, { 7, 8, 9 } };
            range.Value = values;

            // Guarda el libro de trabajo
            workbook.Save("RangePropertyValueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


