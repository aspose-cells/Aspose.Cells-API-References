---
title: "Row.GetCellByIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Row. Obtiene la celda por un índice específico en la colección de celdas de esta fila"
type: docs
url: /es/net/aspose.cells/row/getcellbyindex/
---
## Row.GetCellByIndex method

Obtiene la celda por un índice específico en la colección de celdas de esta fila.

```csharp
public Cell GetCellByIndex(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice (posición) de la celda en la colección de celdas de esta fila. |

### Valor de retorno

El objeto Cell en la posición dada.

### Observaciones

Para recorrer todas las celdas en secuencia sin modificarlas, usar [`GetEnumerator`](../getenumerator/) ofrecerá mejor rendimiento que usar este método para obtener una celda a la vez.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos a las celdas en la primera fila
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            // Obtener la primera fila
            Row row = worksheet.Cells.Rows[0];

            // Demostrar GetCellByIndex con parámetro Int32
            Cell cellAtIndex0 = row.GetCellByIndex(0);
            Cell cellAtIndex1 = row.GetCellByIndex(1);
            Cell cellAtIndex2 = row.GetCellByIndex(2);

            Console.WriteLine("Cell at index 0: " + cellAtIndex0.StringValue);
            Console.WriteLine("Cell at index 1: " + cellAtIndex1.StringValue);
            Console.WriteLine("Cell at index 2: " + cellAtIndex2.StringValue);

            workbook.Save("RowGetCellByIndexDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


