---
title: "Worksheet.GetAdvancedFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Worksheet. Obtiene la configuración del filtro avanzado"
type: docs
url: /es/net/aspose.cells/worksheet/getadvancedfilter/
---
## Worksheet.GetAdvancedFilter method

Obtiene la configuración del filtro avanzado.

```csharp
public AdvancedFilter GetAdvancedFilter()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetAdvancedFilterDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Configurar datos para el filtrado
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Alice");
            sheet.Cells["A4"].PutValue("Bob");
            
            // Configurar rango de criterios
            sheet.Cells["C1"].PutValue("Name");
            sheet.Cells["C2"].PutValue("John");
            
            // Aplicar filtro avanzado
            sheet.AdvancedFilter(true, "A1:A4", "C1:C2", "E1", false);
            
            // Obtener el filtro avanzado
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            
            // Salida de rangos de filtro
            Console.WriteLine("List Range: " + filter.ListRange);
            Console.WriteLine("Criteria Range: " + filter.CriteriaRange);
            Console.WriteLine("Copy To Range: " + filter.CopyToRange);
        }
    }
}
```

### Ver también

* class [AdvancedFilter](../../advancedfilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


