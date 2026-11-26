---
title: "Top10Filter.IsPercent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Top10Filter. Indica si se debe filtrar o no por el valor porcentual de la columna"
type: docs
url: /es/net/aspose.cells/top10filter/ispercent/
---
## Top10Filter.IsPercent property

Indica si se debe filtrar o no por el valor porcentual de la columna

```csharp
public bool IsPercent { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyIsPercentDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue((i + 1) * (j + 1));
                }
            }

            // Aplicar filtro top 10 (no porcentaje)
            worksheet.AutoFilter.Range = "A1:J10";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Obtener el filtro y demostrar la propiedad IsPercent
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output False

            // Aplicar filtro top 10 por porcentaje
            worksheet.AutoFilter.FilterTop10(1, true, true, 20);
            filter = worksheet.AutoFilter.FilterColumns[1].Filter as Top10Filter;
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output True
        }
    }
}
```

### Ver también

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


