---
title: "Row.GetCellOrNull"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Row. Obtiene la celda o null en el índice específico"
type: docs
url: /es/net/aspose.cells/row/getcellornull/
---
## Row.GetCellOrNull method

Obtiene la celda o null en el índice específico.

```csharp
public Cell GetCellOrNull(int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | El índice de columna |

### Valor de retorno

Devuelve el objeto celda si la celda existe. O devuelve null si el objeto celda no existe.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellOrNullWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Agregar datos de ejemplo
            ws.Cells["A1"].PutValue("Header1");
            ws.Cells["B1"].PutValue("Header2");
            ws.Cells["A2"].PutValue(100);
            ws.Cells["B2"].PutValue(200);

            // Obtener la primera fila
            Row row = ws.Cells.Rows[0];

            // Demostrar GetCellOrNull con parámetro Int32
            for (int colIndex = 0; colIndex < 2; colIndex++)
            {
                Cell cell = row.GetCellOrNull(colIndex);
                if (cell != null)
                {
                    Console.WriteLine($"Cell at column {colIndex}: {cell.StringValue}");
                }
                else
                {
                    Console.WriteLine($"Cell at column {colIndex} is null");
                }
            }
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


