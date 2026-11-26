---
title: "FilterColumn.ColorFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FilterColumn. Obtiene ColorFilter para filtrar datos por color"
type: docs
url: /es/net/aspose.cells/filtercolumn/colorfilter/
---
## FilterColumn.ColorFilter property

Obtiene [`ColorFilter`](../../colorfilter/) para filtrar datos por color.

```csharp
public ColorFilter ColorFilter { get; }
```

### Observaciones

Establece [`FilterType`](../filtertype/) como ColorFilter primero, de lo contrario se devolverá Null.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyColorFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Agregar datos de muestra con colores
                worksheet.Cells["A1"].PutValue("Color");
                worksheet.Cells["A2"].PutValue("Red");
                worksheet.Cells["A3"].PutValue("Blue");
                worksheet.Cells["A4"].PutValue("Green");

                // Aplicar filtro automático
                worksheet.AutoFilter.Range = "A1:A4";

                // Obtener la columna de filtro
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Acceder a la propiedad ColorFilter (solo lectura)
                ColorFilter colorFilter = filterColumn.ColorFilter;

                // Mostrar propiedades de ColorFilter
                if (colorFilter != null)
                {
                    Console.WriteLine("ColorFilter is not null");
                    Console.WriteLine("FilterByFillColor: " + colorFilter.FilterByFillColor);
                }
                else
                {
                    Console.WriteLine("ColorFilter is null (no color filter applied)");
                }

                // Guarda el libro de trabajo
                workbook.Save("ColorFilterDemo.xlsx");
                Console.WriteLine("ColorFilter demonstration completed successfully.");
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

* class [ColorFilter](../../colorfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


