---
title: "Cells.ExportArray"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Exporta datos en la colección Cells a un objeto de matriz bidimensional"
type: docs
url: /es/net/aspose.cells/cells/exportarray/
---
## Cells.ExportArray method

Exporta datos en la colección [`Cells`](../) a un objeto de matriz bidimensional.

```csharp
public object[] ExportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | El número de fila de la primera celda a exportar. |
| firstColumn | Int32 | El número de columna de la primera celda a exportar. |
| totalRows | Int32 | Número de filas a exportar |
| totalColumns | Int32 | Número de columnas a exportar |

### Valor de retorno

Objeto de matriz de valores de celda exportado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportArrayWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Poblar algunos datos de muestra
            cells[0, 0].PutValue("A");
            cells[0, 1].PutValue("B");
            cells[1, 0].PutValue(10);
            cells[1, 1].PutValue(20);

            try
            {
                // Exportar datos a una matriz
                object[,] dataArray = cells.ExportArray(0, 0, 2, 2);
                
                // Mostrar la matriz exportada
                for (int i = 0; i < 2; i++)
                {
                    for (int j = 0; j < 2; j++)
                    {
                        Console.Write(dataArray[i, j] + "\t");
                    }
                    Console.WriteLine();
                }
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Error exporting array: " + ex.Message);
            }
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


