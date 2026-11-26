---
title: "AdvancedFilter.ListRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AdvancedFilter. Obtiene el rango de lista de este filtro avanzado"
type: docs
url: /es/net/aspose.cells/advancedfilter/listrange/
---
## AdvancedFilter.ListRange property

Obtiene el rango de lista de este filtro avanzado.

```csharp
public string ListRange { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AdvancedFilterPropertyListRangeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Rellene datos de ejemplo
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Person " + (i-1));
                sheet.Cells["B" + i].PutValue(20 + i);
            }

            // Configurar filtro avanzado
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            // ListRange es de solo lectura y se establece automáticamente al crear el filtro
            // Solo podemos leerlo, no establecerlo directamente
            
            // Mostrar el rango de lista (mostrará el rango determinado automáticamente)
            Console.WriteLine("Advanced Filter List Range: " + filter.ListRange);
            
            // Guarda el libro de trabajo
            workbook.Save("AdvancedFilterDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


