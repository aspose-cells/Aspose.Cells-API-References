---
title: "Range.GetEnumerator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Obtiene el enumerador para las celdas en este rango"
type: docs
url: /es/net/aspose.cells/range/getenumerator/
---
## Range.GetEnumerator method

Obtiene el enumerador de celdas en este Rango.

```csharp
public IEnumerator GetEnumerator()
```

### Valor de retorno

El enumerador de celdas

### Observaciones

Al recorrer los elementos mediante el Enumerator devuelto, la colección de celdas no debe modificarse (por ejemplo, operaciones que provoquen la creación de nuevas Cell/Row o la eliminación de Cell/Row existentes). De lo contrario, el enumerador podría no ser capaz de recorrer todas las celdas correctamente (algunos elementos podrían recorrerse repetidamente o omitirse).

### Ejemplos

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poblar algunos datos de muestra
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Banana");
            worksheet.Cells["C2"].PutValue("Cherry");
            worksheet.Cells["C3"].PutValue("Date");

            // Obtener el rango y enumerar a través de las celdas
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C3");
            IEnumerator enumerator = range.GetEnumerator();
            
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                Console.WriteLine($"{cell.Name}: {cell.Value}");
            }
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


