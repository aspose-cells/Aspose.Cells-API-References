---
title: "Cells.GetEnumerator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el enumerador de celdas"
type: docs
url: /es/net/aspose.cells/cells/getenumerator/
---
## Cells.GetEnumerator method

Obtiene el enumerador de celdas.

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
    public class CellsMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            
            // Obtener el enumerador e iterar a través de las celdas
            IEnumerator enumerator = worksheet.Cells.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                if (cell.Value != null)
                {
                    Console.WriteLine($"{cell.Name}: {cell.Value}");
                }
            }
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


