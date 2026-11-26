---
title: "CellsHelper.ColumnIndexToName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsHelper. Obtiene el nombre de la columna según el índice de columna"
type: docs
url: /es/net/aspose.cells/cellshelper/columnindextoname/
---
## CellsHelper.ColumnIndexToName method

Obtiene el nombre de la columna según el índice de columna.

```csharp
public static string ColumnIndexToName(int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | Índice de columna. |

### Valor de retorno

Nombre de la columna.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodColumnIndexToNameWithInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer valores en celdas para demostrar la conversión de índice de columna a nombre
            worksheet.Cells["A1"].PutValue("Column Index");
            worksheet.Cells["B1"].PutValue("Column Name");

            // Demostrar ColumnIndexToName para los índices 0-4
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(i);
                string columnName = CellsHelper.ColumnIndexToName(i);
                worksheet.Cells[i + 1, 1].PutValue(columnName);
            }

            // Guarda el libro de trabajo
            workbook.Save("ColumnIndexToNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


