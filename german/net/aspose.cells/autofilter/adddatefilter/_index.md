---
title: "AutoFilter.AddDateFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFilter-Methode. Fügt einen Datumsfilter hinzu"
type: docs
url: /de/net/aspose.cells/autofilter/adddatefilter/
---
## AutoFilter.AddDateFilter method

Fügt einen Datumsfilter hinzu.

```csharp
public void AddDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
    int month, int day, int hour, int minute, int second)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldIndex | Int32 | Der ganzzahlige Versatz des Feldes, auf dem der Filter basieren soll (vom linken Rand der Liste; das linkeste Feld ist Feld 0). |
| dateTimeGroupingType | DateTimeGroupingType | Der Gruppierungstyp |
| Jahr | Int32 | Das Jahr. |
| Monat | Int32 | Der Monat. |
| Tag | Int32 | Der Tag. |
| Stunde | Int32 | Die Stunde. |
| Minute | Int32 | Die Minute. |
| Sekunde | Int32 | Die Sekunde. |

### Hinweise

Wenn DateTimeGroupingType Year ist, wirkt nur das Parameter year. Wenn DateTiemGroupingType Month ist, wirken nur die Parameter year und month.

### Beispiele

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

### Siehe auch

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


