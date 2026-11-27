---
title: "DateTimeGroupItem.DateTimeGroupingType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DateTimeGroupItem egenskap. Hämtar och anger grupptypen"
type: docs
url: /sv/net/aspose.cells/datetimegroupitem/datetimegroupingtype/
---
## DateTimeGroupItem.DateTimeGroupingType property

Hämtar och anger grupptypen.

```csharp
public DateTimeGroupingType DateTimeGroupingType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyDateTimeGroupingTypeDemo
    {
        public static void Run()
        {
            // Skapa en instans av DateTimeGroupItem
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year, // Group by Year
                2023,                      // Year
                10,                       // Month
                5,                         // Day
                14,                       // Hour
                30,                       // Minute
                45                        // Second
            );

            // Visa initiala egenskaper
            Console.WriteLine("Initial Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine($"Date Components: {dateTimeGroupItem.Year}-{dateTimeGroupItem.Month}-{dateTimeGroupItem.Day}");

            // Ändra grupperingstyp och datumkomponenter
            dateTimeGroupItem.DateTimeGroupingType = DateTimeGroupingType.Month;
            dateTimeGroupItem.Year = 2022;
            dateTimeGroupItem.Month = 12;

            // Visa modifierade egenskaper
            Console.WriteLine("Modified Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine($"Modified Date Components: {dateTimeGroupItem.Year}-{dateTimeGroupItem.Month}");
        }
    }
}
```

### Se även

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


