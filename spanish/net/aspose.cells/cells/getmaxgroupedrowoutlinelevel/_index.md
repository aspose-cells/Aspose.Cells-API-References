---
title: "Cells.GetMaxGroupedRowOutlineLevel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el nivel de contorno de fila agrupada máximo basado en cero"
type: docs
url: /es/net/aspose.cells/cells/getmaxgroupedrowoutlinelevel/
---
## Cells.GetMaxGroupedRowOutlineLevel method

Obtiene el nivel máximo de esquema de fila agrupada (basado en cero).

```csharp
public int GetMaxGroupedRowOutlineLevel()
```

### Valor de retorno

El nivel de contorno de fila agrupada máximo (basado en cero)

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMaxGroupedRowOutlineLevelDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agrupa algunas filas para demostrar los niveles de contorno
            cells.GroupRows(0, 2, false);
            cells.GroupRows(4, 6, false);
            
            // Agregar agrupación anidada
            cells.GroupRows(4, 5, true);

            // Obtener el nivel de contorno de fila agrupada máximo
            int maxOutlineLevel = cells.GetMaxGroupedRowOutlineLevel();

            // Mostrar el resultado
            Console.WriteLine("Maximum grouped row outline level: " + maxOutlineLevel);

            // Mostrar el nivel de contorno para cada fila
            for (int row = 0; row <= 6; row++)
            {
                Console.WriteLine($"Row {row} outline level: {cells.GetGroupedRowOutlineLevel(row)}");
            }
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


