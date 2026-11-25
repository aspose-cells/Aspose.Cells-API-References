---
title: "DateTimeGroupItem.DateTimeGroupingType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "DateTimeGroupItem proprietà. Ottiene e imposta il tipo di gruppo"
type: docs
url: /it/net/aspose.cells/datetimegroupitem/datetimegroupingtype/
---
## DateTimeGroupItem.DateTimeGroupingType property

Ottiene e imposta il tipo di gruppo.

```csharp
public DateTimeGroupingType DateTimeGroupingType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyDateTimeGroupingTypeDemo
    {
        public static void Run()
        {
            // Crea un'istanza di DateTimeGroupItem
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year, // Group by Year
                2023,                      // Year
                10,                       // Month
                5,                         // Day
                14,                       // Hour
                30,                       // Minute
                45                        // Second
            );

            // Visualizza le proprietà iniziali
            Console.WriteLine("Initial Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine($"Date Components: {dateTimeGroupItem.Year}-{dateTimeGroupItem.Month}-{dateTimeGroupItem.Day}");

            // Modifica il tipo di raggruppamento e i componenti della data
            dateTimeGroupItem.DateTimeGroupingType = DateTimeGroupingType.Month;
            dateTimeGroupItem.Year = 2022;
            dateTimeGroupItem.Month = 12;

            // Visualizza le proprietà modificate
            Console.WriteLine("Modified Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine($"Modified Date Components: {dateTimeGroupItem.Year}-{dateTimeGroupItem.Month}");
        }
    }
}
```

### Vedi anche

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


