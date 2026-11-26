---
title: "FilterColumn.CustomFilters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FilterColumn. Obtiene CustomFilterCollection para filtrar datos por criterios personalizados"
type: docs
url: /es/net/aspose.cells/filtercolumn/customfilters/
---
## FilterColumn.CustomFilters property

Obtiene [`CustomFilterCollection`](../../customfiltercollection/) para filtrar datos por criterios personalizados.

```csharp
public CustomFilterCollection CustomFilters { get; set; }
```

### Observaciones

NOTA: Este setter de esta propiedad está ahora obsoleto. En su lugar, utilice la propiedad [`FilterType`](../filtertype/) configurándola como CustomFilters. Esta propiedad será eliminada 12 meses después desde junio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyCustomFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Agregar datos de ejemplo
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Cherry");
                worksheet.Cells["A5"].PutValue("Date");
                worksheet.Cells["A6"].PutValue("Elderberry");

                // Aplicar filtro automático
                worksheet.AutoFilter.Range = "A1:A6";

                // Obtener la columna de filtro
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Crear y establecer filtros personalizados usando el método AutoFilter.Custom
                // Primer filtro: comienza con "A"
                worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "A", false, FilterOperatorType.None, null);

                // Segundo filtro: termina con "y" (relación AND)
                worksheet.AutoFilter.Custom(0, FilterOperatorType.EndsWith, "y", true, FilterOperatorType.None, null);

                // Obtener los filtros personalizados de la columna de filtro
                CustomFilterCollection customFilters = filterColumn.CustomFilters;

                // Mostrar la información de los filtros personalizados
                Console.WriteLine($"Number of custom filters: {customFilters.Count}");
                Console.WriteLine($"Filter relationship (And): {customFilters.And}");

                // Nota: CustomFilterCollection no expone filtros individuales directamente
                // a través de un indexador, por lo que solo podemos mostrar las propiedades de la colección
                Console.WriteLine("Custom filters have been applied to the column.");

                // Guarda el libro de trabajo
                workbook.Save("CustomFiltersDemo.xlsx");
                Console.WriteLine("CustomFilters demonstration completed successfully.");
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

* class [CustomFilterCollection](../../customfiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


