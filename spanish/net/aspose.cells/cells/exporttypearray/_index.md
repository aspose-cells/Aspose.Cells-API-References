---
title: "Cells.ExportTypeArray"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Exporta el tipo de valor de celda en la colección Cells a un objeto de matriz bidimensional"
type: docs
url: /es/net/aspose.cells/cells/exporttypearray/
---
## Cells.ExportTypeArray method

Exporta el tipo de valor de celda en la colección [`Cells`](../) a un objeto de matriz bidimensional.

```csharp
public CellValueType[] ExportTypeArray(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | El número de fila de la primera celda a exportar. |
| firstColumn | Int32 | El número de columna de la primera celda a exportar. |
| totalRows | Int32 | Número de filas a exportar. |
| totalColumns | Int32 | Número de columnas a exportar. |

### Valor de retorno

Objeto de matriz exportado que representa los tipos de valor de celda.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportTypeArrayWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer valores en celdas
            cells["A1"].PutValue(10);
            cells["B1"].PutValue("Hello");
            cells["A2"].PutValue(true);
            cells["B2"].PutValue(DateTime.Now);

            // Exportar tipos de celda a una matriz 2D
            CellValueType[,] typeArray = cells.ExportTypeArray(0, 0, 2, 2);

            // Muestra los resultados
            for (int i = 0; i < 2; i++)
            {
                for (int j = 0; j < 2; j++)
                {
                    Console.WriteLine($"Cell[{i},{j}] Type: {typeArray[i, j]}");
                }
            }

            // Demostrar caso de excepción
            try
            {
                CellValueType[,] invalidArray = cells.ExportTypeArray(-1, 0, 2, 2);
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Exception caught as expected: " + ex.Message);
            }
        }
    }
}
```

### Ver también

* enum [CellValueType](../../cellvaluetype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


