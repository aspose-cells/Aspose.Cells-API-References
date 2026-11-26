---
title: "FilterColumn.IsDropdownVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FilterColumn. Indica si el botón AutoFilter de esta columna es visible"
type: docs
url: /es/net/aspose.cells/filtercolumn/isdropdownvisible/
---
## FilterColumn.IsDropdownVisible property

Indica si el botón AutoFilter para esta columna es visible.

```csharp
public bool IsDropdownVisible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyIsDropdownVisibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["A4"].PutValue("Fruit");

            // Aplicar AutoFilter
            sheet.AutoFilter.SetRange(0, 0, 3);  // Fixed: Using row/column indices instead of range string

            // Obtener la columna de filtro
            FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

            // Mostrar lista desplegable inicialmente
            filterColumn.IsDropdownVisible = true;
            Console.WriteLine($"Initial IsDropdownVisible: {filterColumn.IsDropdownVisible}");

            // Ocultar la lista desplegable
            filterColumn.IsDropdownVisible = false;
            Console.WriteLine($"After setting to false: {filterColumn.IsDropdownVisible}");

            // Guarda el libro de trabajo
            workbook.Save("FilterColumnDropdownDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


