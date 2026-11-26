---
title: "CellsHelper.CellIndexToName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsHelper. Obtiene el nombre de la celda según sus índices de fila y columna"
type: docs
url: /es/net/aspose.cells/cellshelper/cellindextoname/
---
## CellsHelper.CellIndexToName method

Obtiene el nombre de la celda según sus índices de fila y columna.

```csharp
public static string CellIndexToName(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila. |
| columna | Int32 | Índice de columna. |

### Valor de retorno

Nombre de la celda.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCellIndexToNameWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(20);

            // Obtén el nombre de la celda a partir de los índices de fila y columna
            string cellName = CellsHelper.CellIndexToName(2, 1); // Row 2, Column 1 (B3)

            // Mostrar el resultado
            Console.WriteLine("Cell name for row 2, column 1 is: " + cellName);
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


