---
title: "FilterColumn.DynamicFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FilterColumn. Obtiene DynamicFilter para filtrar con criterios dinámicos"
type: docs
url: /es/net/aspose.cells/filtercolumn/dynamicfilter/
---
## FilterColumn.DynamicFilter property

Obtiene `DynamicFilter` para filtrar con criterios dinámicos.

```csharp
public DynamicFilter DynamicFilter { get; }
```

### Observaciones

Antes de usar esta propiedad, asegúrese de que [`FilterType`](../filtertype/) sea DynamicFilter, de lo contrario se devolverá null.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Agregar datos de ejemplo
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-10));
                worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-5));
                worksheet.Cells["A4"].PutValue(DateTime.Now);

                // Aplicar filtro automático
                worksheet.AutoFilter.Range = "A1:A4";

                // Obtener la columna de filtro
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Acceda a la propiedad DynamicFilter (solo lectura)
                DynamicFilter dynamicFilter = filterColumn.DynamicFilter;

                // Mostrar propiedades de DynamicFilter
                if (dynamicFilter != null)
                {
                    Console.WriteLine("DynamicFilter is not null");
                    Console.WriteLine("DynamicFilterType: " + dynamicFilter.DynamicFilterType);
                    Console.WriteLine("Value: " + dynamicFilter.Value);
                    Console.WriteLine("MaxValue: " + dynamicFilter.MaxValue);
                }
                else
                {
                    Console.WriteLine("DynamicFilter is null (no dynamic filter applied)");
                }

                // Guarda el libro de trabajo
                workbook.Save("DynamicFilterDemo.xlsx");
                Console.WriteLine("DynamicFilter demonstration completed successfully.");
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

* class [DynamicFilter](../../dynamicfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


