---
title: "Top10Filter.IsTop"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Top10Filter. Indica si se debe filtrar o no por orden superior"
type: docs
url: /es/net/aspose.cells/top10filter/istop/
---
## Top10Filter.IsTop property

Indica si se debe filtrar o no por el orden superior

```csharp
public bool IsTop { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyIsTopDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["B6"].PutValue("Value");
            for (int i = 7; i <= 16; i++)
            {
                worksheet.Cells["B" + i].PutValue(20 - i);
            }

            // Aplicar filtro top 5
            worksheet.AutoFilter.Range = "B6:B16";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Obtener el filtro y comprobar la propiedad IsTop
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop); // Should output "True"
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output "False"
            
            // Actualizar el filtro y comprobar filas ocultas
            worksheet.AutoFilter.Refresh();
            for (int i = 6; i <= 16; i++)
            {
                Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### Ver también

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


