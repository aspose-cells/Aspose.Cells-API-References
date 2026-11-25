---
title: "AutoFilter.AddDateFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AutoFilter. Aggiunge un filtro data"
type: docs
url: /it/net/aspose.cells/autofilter/adddatefilter/
---
## AutoFilter.AddDateFilter method

Aggiunge un filtro data.

```csharp
public void AddDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
    int month, int day, int hour, int minute, int second)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | Int32 | L'offset intero del campo su cui si desidera basare il filtro (da sinistra dell'elenco; il campo più a sinistra è il campo 0). |
| dateTimeGroupingType | DateTimeGroupingType | Il tipo di raggruppamento |
| anno | Int32 | L'anno. |
| mese | Int32 | Il mese. |
| giorno | Int32 | Il giorno. |
| ora | Int32 | L'ora. |
| minuto | Int32 | Il minuto. |
| secondo | Int32 | Il secondo. |

### Osservazioni

Se DateTimeGroupingType è Year, solo il parametro year ha effetto. Se DateTiemGroupingType è Month, solo i parametri year e month hanno effetto.

### Esempi

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

### Vedi anche

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


