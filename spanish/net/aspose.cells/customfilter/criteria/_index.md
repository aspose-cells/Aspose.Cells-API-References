---
title: "CustomFilter.Criteria"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CustomFilter. Obtiene y establece los criterios"
type: docs
url: /es/net/aspose.cells/customfilter/criteria/
---
## CustomFilter.Criteria property

Obtiene y establece los criterios.

```csharp
public object Criteria { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomFilterPropertyCriteriaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Numbers");
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(5);
            worksheet.Cells["A5"].PutValue(9);
            worksheet.Cells["A6"].PutValue(3);

            // Aplicar filtro automático
            worksheet.AutoFilter.Range = "A1:A6";
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // Agregar filtro personalizado
            int fieldIndex = 0;
            autoFilter.Custom(fieldIndex, FilterOperatorType.GreaterOrEqual, 5);
            
            // Obtener la columna del filtro y mostrar los criterios
            FilterColumn fc = autoFilter.FilterColumns[fieldIndex];
            CustomFilter cf = ((CustomFilterCollection)fc.Filter)[0];
            Console.WriteLine("Filter Criteria: " + cf.Criteria);
            
            // Actualizar el filtro
            autoFilter.Refresh();
            
            // Guarda el libro de trabajo
            workbook.Save("CustomFilterExample.xlsx");
        }
    }
}
```

### Ver también

* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


