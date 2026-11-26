---
title: "CellsHelper.CellNameToIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsHelper. Obtiene los índices de fila y columna de la celda según su nombre"
type: docs
url: /es/net/aspose.cells/cellshelper/cellnametoindex/
---
## CellsHelper.CellNameToIndex method

Obtiene los índices de fila y columna de la celda según su nombre.

```csharp
public static void CellNameToIndex(string cellName, out int row, out int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String | Nombre de la celda. |
| fila | Int32& | Índice de fila de salida |
| columna | Int32& | Índice de columna de salida |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodCellNameToIndexWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Inicialice variables para contener los índices de fila y columna
            int rowIndex = -1;
            int columnIndex = -1;
            string cellName = "C5";

            try
            {
                // Llame al método CellNameToIndex para convertir el nombre de la celda en índices de fila y columna
                CellsHelper.CellNameToIndex(cellName, out rowIndex, out columnIndex);

                // Muestra los resultados
                Console.WriteLine($"Cell name: {cellName}");
                Console.WriteLine($"Row index: {rowIndex}");
                Console.WriteLine($"Column index: {columnIndex}");

                // Cree un libro de trabajo y demuestre el uso de los índices
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Acceda a la celda usando los índices obtenidos
                Cell cell = worksheet.Cells[rowIndex, columnIndex];
                cell.PutValue("Test Value");

                // Guarda el libro de trabajo
                workbook.Save("CellNameToIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CellNameToIndex method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


