---
title: "DateTimeGroupItem.Day"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "DateTimeGroupItem proprietà. Ottiene e imposta il giorno della data e ora raggruppata"
type: docs
url: /it/net/aspose.cells/datetimegroupitem/day/
---
## DateTimeGroupItem.Day property

Ottiene e imposta il giorno della data/ora raggruppata.

```csharp
public int Day { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyDayDemo
    {
        public static void Run()
        {
            // Crea un DateTimeGroupItem raggruppato per Anno
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,  // Year
                10,    // Month
                5,     // Day
                14,    // Hour
                30,    // Minute
                45     // Second
            );

            // Visualizza il valore iniziale del giorno
            Console.WriteLine("Initial Day: " + dateTimeGroupItem.Day);

            // Modifica la proprietà del giorno
            dateTimeGroupItem.Day = 25;
            Console.WriteLine("Modified Day: " + dateTimeGroupItem.Day);

            // Crea un altro DateTimeGroupItem raggruppato per Day per dimostrare l'importanza della proprietà Day
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

### Vedi anche

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


