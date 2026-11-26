---
title: "Clase Top10Filter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Top10Filter. Representa el N% superior o el número de elementos por los que filtrar"
type: docs
url: /es/net/aspose.cells/top10filter/
---
## Top10Filter class

Representa los N principales (porcentaje o número de elementos) para filtrar.

```csharp
public class Top10Filter
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Criteria](../../aspose.cells/top10filter/criteria/) { get; set; } | (**Obsolete.**) El valor real de la celda en el rango que se utiliza para realizar la comparación para este filtro. Este es el valor en caché durante el proceso de actualización. |
| [IsPercent](../../aspose.cells/top10filter/ispercent/) { get; set; } | Indica si se debe filtrar o no por el valor porcentual de la columna |
| [IsTop](../../aspose.cells/top10filter/istop/) { get; set; } | Indica si se debe filtrar o no por el orden superior |
| [Items](../../aspose.cells/top10filter/items/) { get; set; } | Obtiene y establece el valor superior o inferior a usar como criterio de filtro. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTop10FilterDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["B6"].PutValue("Value");
            for (int i = 7; i <= 16; i++)
            {
                worksheet.Cells["B" + i].PutValue(20 - i);
                worksheet.Cells["C" + i].PutValue("Item " + (i-6));
            }
            
            // Aplicar filtro automático y filtro Top 10
            worksheet.AutoFilter.Range = "B6:C16";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5); // Filter top 5 values in column B
            
            // Obtener el Top10Filter y verificar sus propiedades
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent);
            Console.WriteLine("Items: " + filter.Items);
            
            // Actualizar el filtro y comprobar filas ocultas
            worksheet.AutoFilter.Refresh();
            for (int i = 6; i <= 16; i++)
            {
                Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("Top10FilterDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


