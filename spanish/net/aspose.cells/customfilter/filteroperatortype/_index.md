---
title: "CustomFilter.FilterOperatorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CustomFilter. Obtiene y establece el tipo de operador del filtro"
type: docs
url: /es/net/aspose.cells/customfilter/filteroperatortype/
---
## CustomFilter.FilterOperatorType property

Obtiene y establece el tipo de operador del filtro.

```csharp
public FilterOperatorType FilterOperatorType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomFilterPropertyFilterOperatorTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Names");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Mike");
            worksheet.Cells["A5"].PutValue("Emily");

            // Aplicar filtro automático
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Aplicar filtro personalizado con el operador Contains
            filter.Custom(0, FilterOperatorType.Contains, "e");
            
            // Obtener el primer filtro personalizado
            CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];
            
            // Demostrar la propiedad FilterOperatorType
            Console.WriteLine("Initial Filter Operator: " + customFilter.FilterOperatorType);
            Console.WriteLine("Criteria: " + customFilter.Criteria);
            
            // Cambiar el tipo de operador del filtro
            customFilter.FilterOperatorType = FilterOperatorType.EndsWith;
            Console.WriteLine("Updated Filter Operator: " + customFilter.FilterOperatorType);
            
            // Guarda el libro de trabajo
            workbook.Save("FilterOperatorTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


