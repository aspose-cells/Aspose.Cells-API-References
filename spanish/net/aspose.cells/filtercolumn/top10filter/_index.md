---
title: "FilterColumn.Top10Filter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FilterColumn. Obtiene Top10Filter para filtrar datos por rango de datos"
type: docs
url: /es/net/aspose.cells/filtercolumn/top10filter/
---
## FilterColumn.Top10Filter property

Obtiene `Top10Filter` para filtrar datos por rango de datos.

```csharp
public Top10Filter Top10Filter { get; }
```

### Observaciones

Antes de usar esta propiedad, asegúrese de que [`FilterType`](../filtertype/) sea Top10, de lo contrario se devolverá null.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyTop10FilterDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Poblar algunos datos de muestra
                sheet.Cells["A1"].PutValue("Values");
                sheet.Cells["A2"].PutValue(10);
                sheet.Cells["A3"].PutValue(20);
                sheet.Cells["A4"].PutValue(30);
                sheet.Cells["A5"].PutValue(40);

                // Aplicar un AutoFilter al rango de datos
                sheet.AutoFilter.Range = "A1:A5";

                // Obtener la primera columna de filtro (índice de columna 0)
                FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

                // Mostrar el objeto Filter actual (puede ser null)
                Console.WriteLine("Current Filter object type: " +
                    (filterColumn.Filter != null ? filterColumn.Filter.GetType().FullName : "null"));

                // Verificar si el filtro aplicado es un Top10Filter
                if (filterColumn.Filter != null && filterColumn.Filter.GetType().Name == "Top10Filter")
                {
                    Console.WriteLine("The filter column contains a Top10Filter.");
                }
                else
                {
                    Console.WriteLine("No Top10Filter is applied to this column.");
                }

                // Guardar el libro de trabajo (opcional)
                workbook.Save("Top10FilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Top10Filter](../../top10filter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


