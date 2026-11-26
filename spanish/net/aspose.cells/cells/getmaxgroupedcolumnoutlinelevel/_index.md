---
title: "Cells.GetMaxGroupedColumnOutlineLevel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Obtiene el nivel de contorno de columna agrupada máximo, basado en cero"
type: docs
url: /es/net/aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/
---
## Cells.GetMaxGroupedColumnOutlineLevel method

Obtiene el nivel máximo de esquema de columna agrupada (basado en cero).

```csharp
public int GetMaxGroupedColumnOutlineLevel()
```

### Valor de retorno

El nivel de contorno de columna agrupada máximo (basado en cero)

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMaxGroupedColumnOutlineLevelDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agrupar algunas columnas para demostrar los niveles de contorno
            cells.GroupColumns(0, 2, false);
            cells.GroupColumns(3, 5, false);
            
            // Obtener el nivel de contorno de columna agrupada máximo
            int maxOutlineLevel = cells.GetMaxGroupedColumnOutlineLevel();
            
            Console.WriteLine("Maximum grouped column outline level: " + maxOutlineLevel);
            
            // Mostrar el nivel de contorno para cada columna
            for (int col = 0; col < 6; col++)
            {
                int outlineLevel = cells.GetGroupedColumnOutlineLevel(col);
                Console.WriteLine($"Column {col} outline level: {outlineLevel}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("GroupedColumnsOutlineLevel.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


