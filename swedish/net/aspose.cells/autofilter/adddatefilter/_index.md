---
title: "AutoFilter.AddDateFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoFilter-metod. Lägger till ett datumfilter"
type: docs
url: /sv/net/aspose.cells/autofilter/adddatefilter/
---
## AutoFilter.AddDateFilter method

Lägger till ett datumfilter.

```csharp
public void AddDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
    int month, int day, int hour, int minute, int second)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | Int32 | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstra fältet är fält 0). |
| dateTimeGroupingType | DateTimeGroupingType | Grupperingstypen |
| år | Int32 | Året. |
| månad | Int32 | Månaden. |
| dag | Int32 | Dagen. |
| timme | Int32 | Timmen. |
| minut | Int32 | Minuten. |
| sekund | Int32 | Sekunden. |

### Anmärkningar

Om DateTimeGroupingType är Year, påverkar bara parametern year. Om DateTiemGroupingType är Month, påverkar bara parametrarna year och month.

### Exempel

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

### Se även

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


