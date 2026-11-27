---
title: "DateTimeGroupItem.MinValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DateTimeGroupItem-egenskap. Hämtar minvärdet"
type: docs
url: /sv/net/aspose.cells/datetimegroupitem/minvalue/
---
## DateTimeGroupItem.MinValue property

Hämtar minvärdet.

```csharp
public DateTime MinValue { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMinValueDemo
    {
        public static void Run()
        {
            // Skapa en instans av DateTimeGroupItem
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year, // Group by Year
                2023,                      // Year
                10,                        // Month
                5,                         // Day
                14,                        // Hour
                30,                        // Minute
                45                         // Second
            );

            // Demonstrera MinValue-egenskapen
            Console.WriteLine("MinValue: " + dateTimeGroupItem.MinValue);

            // Visa andra egenskaper för sammanhang
            Console.WriteLine("Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Date Components: {0}-{1}-{2} {3}:{4}:{5}",
                dateTimeGroupItem.Year,
                dateTimeGroupItem.Month,
                dateTimeGroupItem.Day,
                dateTimeGroupItem.Hour,
                dateTimeGroupItem.Minute,
                dateTimeGroupItem.Second);
        }
    }
}
```

### Se även

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


