---
title: "DateTimeGroupItem.Day"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DateTimeGroupItem egenskap. Hämtar och anger dagen för den grupperade datum-tiden"
type: docs
url: /sv/net/aspose.cells/datetimegroupitem/day/
---
## DateTimeGroupItem.Day property

Hämtar och anger dagen i den grupperade datum/tiden.

```csharp
public int Day { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyDayDemo
    {
        public static void Run()
        {
            // Skapa ett DateTimeGroupItem grupperat efter år
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,  // Year
                10,    // Month
                5,     // Day
                14,    // Hour
                30,    // Minute
                45     // Second
            );

            // Visa initialt dagvärde
            Console.WriteLine("Initial Day: " + dateTimeGroupItem.Day);

            // Ändra dag-egenskapen
            dateTimeGroupItem.Day = 25;
            Console.WriteLine("Modified Day: " + dateTimeGroupItem.Day);

            // Skapa ett annat DateTimeGroupItem grupperat efter Dag för att demonstrera betydelsen av Dag-egenskapen
            DateTimeGroupItem dayGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Day,
                2023,
                10,
                15,  // Initial day
                0,
                0,
                0
            );

            Console.WriteLine("\nDay-grouped item initial Day: " + dayGroupItem.Day);
            dayGroupItem.Day = 20;
            Console.WriteLine("Day-grouped item modified Day: " + dayGroupItem.Day);
        }
    }
}
```

### Se även

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


