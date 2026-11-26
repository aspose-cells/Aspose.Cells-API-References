---
title: "Cells.GetGroupedRowOutlineLevel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el nivel de contorno basado en cero de la fila"
type: docs
url: /es/net/aspose.cells/cells/getgroupedrowoutlinelevel/
---
## Cells.GetGroupedRowOutlineLevel method

Obtiene el nivel de esquema (basado en cero) de la fila.

```csharp
public int GetGroupedRowOutlineLevel(int rowIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | El índice de fila. |

### Valor de retorno

El nivel de contorno (basado en cero) de la fila.

### Observaciones

Si la fila no está agrupada, devuelve cero.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetGroupedRowOutlineLevelWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agrupar filas 0-3 (nivel 1)
            cells.GroupRows(0, 3, false);
            
            // Agrupar filas 0-1 (nivel 2)
            cells.GroupRows(0, 1, false);

            // Obtener el nivel de contorno para cada fila
            for (int row = 0; row <= 4; row++)
            {
                int outlineLevel = cells.GetGroupedRowOutlineLevel(row);
                Console.WriteLine($"Row {row} outline level: {outlineLevel}");
            }

            // Desagrupar todas las filas
            cells.UngroupRows(0, 3);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


