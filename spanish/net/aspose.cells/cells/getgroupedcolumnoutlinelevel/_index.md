---
title: "Cells.GetGroupedColumnOutlineLevel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el nivel de contorno basado en cero de la columna"
type: docs
url: /es/net/aspose.cells/cells/getgroupedcolumnoutlinelevel/
---
## Cells.GetGroupedColumnOutlineLevel method

Obtiene el nivel de esquema (basado en cero) de la columna.

```csharp
public int GetGroupedColumnOutlineLevel(int columnIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnIndex | Int32 | El índice de columna |

### Valor de retorno

El nivel de contorno de la columna

### Observaciones

Si la columna no está agrupada, devuelve cero.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetGroupedColumnOutlineLevelWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrupar columnas (primeras 3 columnas) sin ocultarlas
            worksheet.Cells.GroupColumns(0, 2, false);
            
            // Obtener nivel de esquema de la primera columna
            int outlineLevel = worksheet.Cells.GetGroupedColumnOutlineLevel(0);
            
            Console.WriteLine("Outline level of column 0: " + outlineLevel);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


