---
title: "DateTimeGroupItem.Month"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DateTimeGroupItem-egenskap. Hämtar och sätter månaden för den grupperade datumtiden"
type: docs
url: /sv/net/aspose.cells/datetimegroupitem/month/
---
## DateTimeGroupItem.Month property

Hämtar och anger månaden i den grupperade datum/tiden.

```csharp
public int Month { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMonthDemo
    {
        public static void Run()
        {
            // Skapa ett DateTimeGroupItem grupperat efter Month
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Month,
                2023,
                10,
                1,
                0,
                0,
                0
            );

            // Visa initialt månadsvärde
            Console.WriteLine("Initial Month: " + dateTimeGroupItem.Month);

            // Ändra månadsvärdet
            dateTimeGroupItem.Month = 12;
            Console.WriteLine("Modified Month: " + dateTimeGroupItem.Month);

            // Skapa ett annat DateTimeGroupItem med annan gruppering
            DateTimeGroupItem yearlyItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,
                1,
                1,
                0,
                0,
                0
            );

            // Visa att Month-egenskapen fortfarande är åtkomlig även när den är grupperad efter Year
            Console.WriteLine("Yearly Grouping - Month: " + yearlyItem.Month);
        }
    }
}
```

### Se även

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


