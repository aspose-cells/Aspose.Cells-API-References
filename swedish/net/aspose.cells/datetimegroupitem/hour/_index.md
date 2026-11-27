---
title: "DateTimeGroupItem.Hour"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DateTimeGroupItem‑egenskap. Hämtar och anger timmen för den grupperade datumtiden"
type: docs
url: /sv/net/aspose.cells/datetimegroupitem/hour/
---
## DateTimeGroupItem.Hour property

Hämtar och anger timmen i den grupperade datum/tiden.

```csharp
public int Hour { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyHourDemo
    {
        public static void Run()
        {
            // Skapa ett DateTimeGroupItem med timmegruppering
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Hour,
                2023,  // Year
                10,     // Month
                5,      // Day
                14,     // Hour
                0,      // Minute
                0      // Second
            );

            // Visa ursprungligt timvärde
            Console.WriteLine("Initial Hour: " + dateTimeGroupItem.Hour);

            // Ändra timme‑egenskapen
            dateTimeGroupItem.Hour = 18;

            // Visa modifierat timvärde
            Console.WriteLine("Modified Hour: " + dateTimeGroupItem.Hour);
        }
    }
}
```

### Se även

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


