---
title: "Enum DateTimeGroupingType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DateTimeGroupingType enum. Anger hur dateTime‑värden ska grupperas"
type: docs
url: /sv/net/aspose.cells/datetimegroupingtype/
---
## DateTimeGroupingType enumeration

Anger hur datum/tid‑värden ska grupperas.

```csharp
public enum DateTimeGroupingType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Day | `0` | Gruppera efter dag. |
| Hour | `1` | Gruppera efter timme. |
| Minute | `2` | Gruppera efter minut. |
| Month | `3` | Gruppera efter månad. |
| Second | `4` | Gruppera efter sekund. |
| Year | `5` | Gruppera efter år. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupingTypeDemo
    {
        public static void DateTimeGroupingTypeExample()
        {
            // Skapar en arbetsbok och får åtkomst till det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägger till exempeldata
            worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1, 10, 0, 0));
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1, 11, 0, 0));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2, 10, 0, 0));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 1, 2, 11, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 2, 1, 10, 0, 0));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 2, 1, 11, 0, 0));

            // Skapar ett AutoFilter och anger intervallet
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:A6";

            // Lägger till datumfilter med olika DateTimeGroupingType
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Month, 2023, 1, 1, 0, 0, 0);
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Hour, 2023, 1, 1, 10, 0, 0);
            
            // Sparar arbetsboken
            workbook.Save("DateTimeGroupingTypeExample.xlsx");
            workbook.Save("DateTimeGroupingTypeExample.pdf");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


