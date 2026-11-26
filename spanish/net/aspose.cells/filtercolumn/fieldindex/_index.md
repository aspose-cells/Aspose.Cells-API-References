---
title: "FilterColumn.FieldIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FilterColumn. Obtiene y establece el desplazamiento de columna en el rango"
type: docs
url: /es/net/aspose.cells/filtercolumn/fieldindex/
---
## FilterColumn.FieldIndex property

Obtiene y establece el desplazamiento de columna en el rango.

```csharp
public int FieldIndex { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Department");
            worksheet.Cells["B1"].PutValue("Employees");
            worksheet.Cells["A2"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["A3"].PutValue("Marketing");
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["A4"].PutValue("IT");
            worksheet.Cells["B4"].PutValue(12);

            // Aplicar filtro automático
            worksheet.AutoFilter.Range = "A1:B4";
            
            // Agregar filtro a la primera columna (Departamento)
            worksheet.AutoFilter.AddFilter(0, "Sales");

            // Obtener la columna de filtro
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            
            // Demostrar la propiedad FieldIndex
            Console.WriteLine("Filter is applied on column index: " + filterColumn.FieldIndex);
            
            // Actualizar y guardar
            worksheet.AutoFilter.Refresh();
            workbook.Save("FilterColumnFieldIndexDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


