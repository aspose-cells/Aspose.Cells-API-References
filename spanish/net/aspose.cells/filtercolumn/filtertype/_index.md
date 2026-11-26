---
title: "FilterColumn.FilterType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FilterColumn. Obtiene y establece el tipo de filtrado de datos"
type: docs
url: /es/net/aspose.cells/filtercolumn/filtertype/
---
## FilterColumn.FilterType property

Obtiene y establece el tipo de filtrado de datos.

```csharp
public FilterType FilterType { get; set; }
```

### Observaciones

El objeto de filtro correspondiente se creará cuando se establezca esta propiedad y la propiedad correspondiente debe usarse para obtener el objeto de filtro en consecuencia:

| **FilterType** | **Property** |
| --- | --- |
| MultipleFilters | [`FilterValues`](../filtervalues/) |
| CustomFilters | [`CustomFilters`](../customfilters/) |
| ColorFilter | [`ColorFilter`](../colorfilter/) |
| DynamicFilter | [`DynamicFilter`](../dynamicfilter/) |
| IconFilter | [`IconFilter`](../iconfilter/) |
| Top10 | [`Top10Filter`](../top10filter/) |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFilterTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Department");
            sheet.Cells["A2"].PutValue("HR");
            sheet.Cells["A3"].PutValue("IT");
            sheet.Cells["A4"].PutValue("Finance");

            sheet.Cells["B1"].PutValue("Employees");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(15);
            sheet.Cells["B4"].PutValue(8);

            // Aplicar filtro automático usando rango de cadena
            sheet.AutoFilter.Range = "A1:B4";

            // Agregar diferentes tipos de filtro para demostrar la propiedad FilterType
            sheet.AutoFilter.AddFilter(0, "HR"); // Simple filter
            sheet.AutoFilter.Custom(1, FilterOperatorType.GreaterThan, 10); // Custom filter

            // Obtener columnas de filtro
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // Mostrar FilterType para cada columna
            for (int i = 0; i < filterColumns.Count; i++)
            {
                FilterColumn filterColumn = filterColumns[i];
                Console.WriteLine($"Column {i} FilterType: {filterColumn.FilterType}");
            }

            // Guarda el libro de trabajo
            workbook.Save("FilterTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FilterType](../../filtertype/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


