---
title: "DateTimeGroupItem.Year"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DateTimeGroupItem‑egenskap. Hämtar och anger året för den grupperade datumtiden"
type: docs
url: /sv/net/aspose.cells/datetimegroupitem/year/
---
## DateTimeGroupItem.Year property

Hämtar och anger året för den grupperade datum/tiden.

```csharp
public int Year { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyYearDemo
    {
        public static void Run()
        {
            // Skapa ett DateTimeGroupItem grupperat efter år
            DateTimeGroupItem dateTimeGroup = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,  // Year
                1,     // Month (ignored when grouping by Year)
                1,     // Day (ignored)
                0,     // Hour (ignored)
                0,     // Minute (ignored)
                0      // Second (ignored)
            );

            // Visa ursprungligt årvärde
            Console.WriteLine("Initial Year: " + dateTimeGroup.Year);

            // Ändra år‑egenskapen
            dateTimeGroup.Year = 2024;

            // Visa modifierat årvärde
            Console.WriteLine("Modified Year: " + dateTimeGroup.Year);

            // Visa att andra egenskaper ignoreras vid gruppering efter år
            dateTimeGroup.Month = 12;
            Console.WriteLine("Month value is ignored when grouping by Year: " + dateTimeGroup.Month);
        }
    }
}
```

### Se även

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


