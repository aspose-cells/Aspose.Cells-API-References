---
title: "DateTimeGroupItem.Minute"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DateTimeGroupItem egenskap. Hämtar och anger minuten för den grupperade datum-tiden"
type: docs
url: /sv/net/aspose.cells/datetimegroupitem/minute/
---
## DateTimeGroupItem.Minute property

Hämtar och anger minuten i den grupperade datum/tiden.

```csharp
public int Minute { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMinuteDemo
    {
        public static void Run()
        {
            // Skapa ett DateTimeGroupItem med initiala värden
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,
                10,
                5,
                14,
                30,
                45
            );

            // Visa initialt minutvärde
            Console.WriteLine("Initial Minute: " + dateTimeGroupItem.Minute);

            // Ändra minutvärdet
            dateTimeGroupItem.Minute = 15;

            // Visa modifierat minutvärde
            Console.WriteLine("Modified Minute: " + dateTimeGroupItem.Minute);

            // Skapa ett nytt DateTimeGroupItem med endast minutgruppering
            DateTimeGroupItem minuteGroup = new DateTimeGroupItem(
                DateTimeGroupingType.Minute,
                0, 0, 0, 0, 45, 0
            );

            // Visa minut från minutgruppering
            Console.WriteLine("Minute from Minute Grouping: " + minuteGroup.Minute);
        }
    }
}
```

### Se även

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


