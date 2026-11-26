---
title: "AutoFilter.FilterColumns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AutoFilter. Obtiene la colección de columnas de filtro"
type: docs
url: /es/net/aspose.cells/autofilter/filtercolumns/
---
## AutoFilter.FilterColumns property

Obtiene la colección de columnas de filtro.

```csharp
public FilterColumnCollection FilterColumns { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterPropertyFilterColumnsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Department");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Status");
            
            worksheet.Cells["A2"].PutValue("HR");
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["C2"].PutValue("Present");
            
            worksheet.Cells["A3"].PutValue("IT");
            worksheet.Cells["B3"].PutValue("Sarah");
            worksheet.Cells["C3"].PutValue("Absent");
            
            worksheet.Cells["A4"].PutValue("HR");
            worksheet.Cells["B4"].PutValue("Mike");
            worksheet.Cells["C4"].PutValue("Present");

            // Aplicar filtro automático
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:C1";
            
            // Filtrar columna 2 (Status) para valores "Present"
            autoFilter.Filter(2, "Present");
            
            // Acceder a la columna de filtro
            FilterColumn filterColumn = autoFilter.FilterColumns[2];
            
            // Guarda el libro de trabajo
            workbook.Save("AutoFilterExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [FilterColumnCollection](../../filtercolumncollection/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


