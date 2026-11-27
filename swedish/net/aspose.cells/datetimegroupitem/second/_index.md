---
title: "DateTimeGroupItem.Second"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DateTimeGroupItem-egenskap. Hämtar och sätter sekunden för den grupperade datumtiden"
type: docs
url: /sv/net/aspose.cells/datetimegroupitem/second/
---
## DateTimeGroupItem.Second property

Hämtar och anger sekunden i den grupperade datum/tiden.

```csharp
public int Second { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertySecondDemo
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

            // Visa initialt sekundvärde
            Console.WriteLine("Initial Second: " + dateTimeGroupItem.Second);

            // Modifiera sekundvärdet
            dateTimeGroupItem.Second = 50;
            Console.WriteLine("Modified Second: " + dateTimeGroupItem.Second);

            // Skapa en annan instans med annat sekundvärde
            DateTimeGroupItem anotherItem = new DateTimeGroupItem(
                DateTimeGroupingType.Day,
                2023,
                10,
                5,
                14,
                30,
                0  // Second set to 0
            );
            Console.WriteLine("Another Item Second: " + anotherItem.Second);
        }
    }
}
```

### Se även

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


