---
title: "Enumeración DateTimeGroupingType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.DateTimeGroupingType. Especifica cómo agrupar valores de fecha y hora"
type: docs
url: /es/net/aspose.cells/datetimegroupingtype/
---
## DateTimeGroupingType enumeration

Especifica cómo agrupar valores de fecha y hora.

```csharp
public enum DateTimeGroupingType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Day | `0` | Agrupar por día. |
| Hour | `1` | Agrupar por hora. |
| Minute | `2` | Agrupar por minuto. |
| Month | `3` | Agrupar por mes. |
| Second | `4` | Agrupar por segundo. |
| Year | `5` | Agrupar por año. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupingTypeDemo
    {
        public static void DateTimeGroupingTypeExample()
        {
            // Creando un libro de trabajo y accediendo a la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregando algunos datos de muestra
            worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1, 10, 0, 0));
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1, 11, 0, 0));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2, 10, 0, 0));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 1, 2, 11, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 2, 1, 10, 0, 0));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 2, 1, 11, 0, 0));

            // Creando un AutoFiltro y estableciendo el rango
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:A6";

            // Agregando filtros de fecha con diferentes DateTimeGroupingType
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Month, 2023, 1, 1, 0, 0, 0);
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Hour, 2023, 1, 1, 10, 0, 0);
            
            // Guardando el libro de trabajo
            workbook.Save("DateTimeGroupingTypeExample.xlsx");
            workbook.Save("DateTimeGroupingTypeExample.pdf");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


