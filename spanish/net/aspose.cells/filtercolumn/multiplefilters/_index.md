---
title: "FilterColumn.MultipleFilters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FilterColumn. Obtiene MultipleFilterCollection para filtrar datos por etiquetas o fecha y hora"
type: docs
url: /es/net/aspose.cells/filtercolumn/multiplefilters/
---
## FilterColumn.MultipleFilters property

Obtiene [`MultipleFilterCollection`](../../multiplefiltercollection/) para filtrar datos por etiquetas o fecha y hora.

```csharp
[Obsolete("Use FilterColumn.FilterValues instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MultipleFilterCollection MultipleFilters { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad FilterColumn.FilterValues. Esta propiedad será eliminada 12 meses después, a partir de junio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyMultipleFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Agregar datos de ejemplo
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("Fruit");
                worksheet.Cells["A3"].PutValue("Vegetable");
                worksheet.Cells["A4"].PutValue("Fruit");
                worksheet.Cells["A5"].PutValue("Grain");

                // Aplicar AutoFilter al rango
                worksheet.AutoFilter.Range = "A1:A5";

                // Obtener la primera columna de filtro
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Crear y establecer MultipleFilters
                MultipleFilterCollection multipleFilters = new MultipleFilterCollection();
                multipleFilters.Add("Fruit");
                multipleFilters.Add("Vegetable");
                multipleFilters.MatchBlank = false;

                // Asignar los MultipleFilters a la columna de filtro
                filterColumn.MultipleFilters = multipleFilters;

                // Mostrar las propiedades de MultipleFilters
                Console.WriteLine("MultipleFilters Count: " + filterColumn.MultipleFilters.Count);
                Console.WriteLine("MatchBlank: " + filterColumn.MultipleFilters.MatchBlank);

                // Guarda el libro de trabajo
                workbook.Save("MultipleFiltersDemo.xlsx");
                Console.WriteLine("MultipleFilters demonstration completed successfully.");
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

* class [MultipleFilterCollection](../../multiplefiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


