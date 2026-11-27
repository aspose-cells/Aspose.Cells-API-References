---
title: "Klassen DateTimeGroupItem"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Klassen Aspose.Cells.DateTimeGroupItem. Representerar datum/tid-gruppinställningen"
type: docs
url: /sv/net/aspose.cells/datetimegroupitem/
---
## DateTimeGroupItem class

Representerar datum/tid-gruppinställningen.

```csharp
public class DateTimeGroupItem
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [DateTimeGroupItem](datetimegroupitem/)(DateTimeGroupingType, int, int, int, int, int, int) |  |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [DateTimeGroupingType](../../aspose.cells/datetimegroupitem/datetimegroupingtype/) { get; set; } | Hämtar och anger grupptypen. |
| [Day](../../aspose.cells/datetimegroupitem/day/) { get; set; } | Hämtar och anger dagen i den grupperade datum/tiden. |
| [Hour](../../aspose.cells/datetimegroupitem/hour/) { get; set; } | Hämtar och anger timmen i den grupperade datum/tiden. |
| [Minute](../../aspose.cells/datetimegroupitem/minute/) { get; set; } | Hämtar och anger minuten i den grupperade datum/tiden. |
| [MinValue](../../aspose.cells/datetimegroupitem/minvalue/) { get; } | Hämtar minvärdet. |
| [Month](../../aspose.cells/datetimegroupitem/month/) { get; set; } | Hämtar och anger månaden i den grupperade datum/tiden. |
| [Second](../../aspose.cells/datetimegroupitem/second/) { get; set; } | Hämtar och anger sekunden i den grupperade datum/tiden. |
| [Year](../../aspose.cells/datetimegroupitem/year/) { get; set; } | Hämtar och anger året för den grupperade datum/tiden. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupItemDemo
    {
        public static void DateTimeGroupItemExample()
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

            // Åtkomst till egenskaper
            Console.WriteLine("MinValue: " + dateTimeGroupItem.MinValue);
            Console.WriteLine("DateTimeGroupingType: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Year: " + dateTimeGroupItem.Year);
            Console.WriteLine("Month: " + dateTimeGroupItem.Month);
            Console.WriteLine("Day: " + dateTimeGroupItem.Day);
            Console.WriteLine("Hour: " + dateTimeGroupItem.Hour);
            Console.WriteLine("Minute: " + dateTimeGroupItem.Minute);
            Console.WriteLine("Second: " + dateTimeGroupItem.Second);

            // Modifierar egenskaper
            dateTimeGroupItem.DateTimeGroupingType = DateTimeGroupingType.Month;
            dateTimeGroupItem.Year = 2022;
            dateTimeGroupItem.Month = 12;
            dateTimeGroupItem.Day = 25;
            dateTimeGroupItem.Hour = 10;
            dateTimeGroupItem.Minute = 15;
            dateTimeGroupItem.Second = 30;

            // Åtkomst till modifierade egenskaper
            Console.WriteLine("Modified DateTimeGroupingType: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Modified Year: " + dateTimeGroupItem.Year);
            Console.WriteLine("Modified Month: " + dateTimeGroupItem.Month);
            Console.WriteLine("Modified Day: " + dateTimeGroupItem.Day);
            Console.WriteLine("Modified Hour: " + dateTimeGroupItem.Hour);
            Console.WriteLine("Modified Minute: " + dateTimeGroupItem.Minute);
            Console.WriteLine("Modified Second: " + dateTimeGroupItem.Second);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


