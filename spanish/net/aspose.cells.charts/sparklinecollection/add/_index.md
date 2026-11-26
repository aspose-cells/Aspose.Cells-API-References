---
title: "SparklineCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SparklineCollection. Añade un sparkline"
type: docs
url: /es/net/aspose.cells.charts/sparklinecollection/add/
---
## SparklineCollection.Add method

Agregar una sparkline.

```csharp
public int Add(string dataRange, int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataRange | String | Especifica el nuevo rango de datos del sparkline. |
| fila | Int32 | El índice de fila de la ubicación. |
| columna | Int32 | El índice de columna de la ubicación. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineCollectionMethodAddWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            for (int i = 0; i < 12; i++)
            {
                worksheet.Cells[4, 3 + i].PutValue(i + 1);
            }

            // Crear un grupo de sparkline
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Añadir sparkline con rango de datos y ubicación
            int sparklineIndex = group.Sparklines.Add("D5:O5", 4, 15);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


