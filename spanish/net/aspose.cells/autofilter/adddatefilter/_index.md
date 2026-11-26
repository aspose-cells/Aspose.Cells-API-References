---
title: "AutoFilter.AddDateFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AutoFilter. Añade un filtro de fecha"
type: docs
url: /es/net/aspose.cells/autofilter/adddatefilter/
---
## AutoFilter.AddDateFilter method

Añade un filtro de fecha.

```csharp
public void AddDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
    int month, int day, int hour, int minute, int second)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | Int32 | El desplazamiento entero del campo sobre el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| dateTimeGroupingType | DateTimeGroupingType | El tipo de agrupación |
| año | Int32 | El año. |
| mes | Int32 | El mes. |
| día | Int32 | El día. |
| hora | Int32 | La hora. |
| minuto | Int32 | El minuto. |
| segundo | Int32 | El segundo. |

### Observaciones

Si DateTimeGroupingType es Year, solo el parámetro year tiene efecto. Si DateTiemGroupingType es Month, solo los parámetros year y month tienen efecto.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodAddDateFilterWithInt32DateTimeGroupingTypeInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1, 10, 0, 0));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 1, 1, 11, 0, 0));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 1, 2, 10, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 2, 1, 10, 0, 0));

            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:A5";

            autoFilter.AddDateFilter(0, DateTimeGroupingType.Month, 2023, 1, 1, 0, 0, 0);
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Day, 2023, 1, 2, 0, 0, 0);

            workbook.Save("AutoFilterAddDateFilterExample.xlsx");
        }
    }
}
```

### Ver también

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


