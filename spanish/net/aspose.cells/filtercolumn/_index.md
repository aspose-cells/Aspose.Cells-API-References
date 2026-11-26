---
title: "Clase FilterColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.FilterColumn. Representa un filtro para una sola columna o una columna en la tabla"
type: docs
url: /es/net/aspose.cells/filtercolumn/
---
## FilterColumn class

Representa un filtro para una sola columna o una columna en la tabla.

```csharp
public class FilterColumn
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ColorFilter](../../aspose.cells/filtercolumn/colorfilter/) { get; } | Obtiene [`ColorFilter`](../colorfilter/) para filtrar datos por color. |
| [CustomFilters](../../aspose.cells/filtercolumn/customfilters/) { get; set; } | Obtiene [`CustomFilterCollection`](../customfiltercollection/) para filtrar datos por criterios personalizados. |
| [DynamicFilter](../../aspose.cells/filtercolumn/dynamicfilter/) { get; } | Obtiene [`DynamicFilter`](./dynamicfilter/) para filtrar con criterios dinámicos. |
| [FieldIndex](../../aspose.cells/filtercolumn/fieldindex/) { get; set; } | Obtiene y establece el desplazamiento de columna en el rango. |
| [Filter](../../aspose.cells/filtercolumn/filter/) { get; set; } | (**Obsoleto.**) Obtiene y establece la condición del filtrado de datos. |
| [FilterType](../../aspose.cells/filtercolumn/filtertype/) { get; set; } | Obtiene y establece el tipo de filtrado de datos. |
| [FilterValues](../../aspose.cells/filtercolumn/filtervalues/) { get; } | Obtiene [`FilterValueCollection`](../filtervaluecollection/) para filtrar datos por etiquetas o fecha y hora. |
| [IconFilter](../../aspose.cells/filtercolumn/iconfilter/) { get; } | Obtiene [`IconFilter`](./iconfilter/) para filtrar datos por ícono. |
| [IsDropdownVisible](../../aspose.cells/filtercolumn/isdropdownvisible/) { get; set; } | Indica si el botón AutoFilter para esta columna es visible. |
| [MultipleFilters](../../aspose.cells/filtercolumn/multiplefilters/) { get; set; } | (**Obsoleto.**) Obtiene [`MultipleFilterCollection`](../multiplefiltercollection/) para filtrar datos por etiquetas o fecha y hora. |
| [Top10Filter](../../aspose.cells/filtercolumn/top10filter/) { get; } | Obtiene [`Top10Filter`](./top10filter/) para filtrar datos por rango de datos. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SelectAll](../../aspose.cells/filtercolumn/selectall/)() | Selecciona todo. |

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;

namespace AsposeCellsExamples
{
    public class FilterColumnDemo
    {
        public static void RunDemo()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Jane");
            sheet.Cells["A4"].PutValue("Doe");

            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(25);
            sheet.Cells["B4"].PutValue(35);

            // Aplicar AutoFilter al rango
            sheet.AutoFilter.SetRange(0, 0, 3);

            // Agregar un filtro a la primera columna (Name)
            sheet.AutoFilter.AddFilter(0, "John");

            // Agregar un filtro a la segunda columna (Age)
            sheet.AutoFilter.AddFilter(1, "30");

            // Actualizar el filtro para aplicarlo
            sheet.AutoFilter.Refresh();

            // Acceder a la colección FilterColumnCollection
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // Acceder al primer FilterColumn
            FilterColumn filterColumn = filterColumns[0];

            // Mostrar propiedades del FilterColumn
            Console.WriteLine($"IsDropdownVisible: {filterColumn.IsDropdownVisible}");
            Console.WriteLine($"Filter: {filterColumn.Filter}");
            Console.WriteLine($"FilterType: {filterColumn.FilterType}");
            Console.WriteLine($"FieldIndex: {filterColumn.FieldIndex}");

            // Guarda el libro de trabajo
            workbook.Save("FilterColumnDemo.xlsx");
            workbook.Save("FilterColumnDemo.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


