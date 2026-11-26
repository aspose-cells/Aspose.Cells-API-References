---
title: "Cells.HideRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Oculta varias filas"
type: docs
url: /es/net/aspose.cells/cells/hiderows/
---
## Cells.HideRows method

Oculta varias filas.

```csharp
public void HideRows(int row, int totalRows)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila. |
| totalRows | Int32 | El número de fila. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].Value = $"Row {i+1}, Col {j+1}";
                }
            }

            // Ocultar filas 3 a 5 (índice basado en 0: 2 a 4)
            worksheet.Cells.HideRows(2, 3);

            // Guarda el libro de trabajo
            workbook.Save("HideRowsExample.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


