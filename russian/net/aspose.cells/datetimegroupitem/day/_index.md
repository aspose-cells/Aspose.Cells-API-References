---
title: "DateTimeGroupItem.Day"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DateTimeGroupItem. Получает и задает день сгруппированного даты и времени"
type: docs
url: /ru/net/aspose.cells/datetimegroupitem/day/
---
## DateTimeGroupItem.Day property

Получает и задаёт день сгруппированной даты и времени.

```csharp
public int Day { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyDayDemo
    {
        public static void Run()
        {
            // Создать DateTimeGroupItem, сгруппированный по году
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,  // Year
                10,    // Month
                5,     // Day
                14,    // Hour
                30,    // Minute
                45     // Second
            );

            // Отобразить начальное значение дня
            Console.WriteLine("Initial Day: " + dateTimeGroupItem.Day);

            // Изменить свойство дня
            dateTimeGroupItem.Day = 25;
            Console.WriteLine("Modified Day: " + dateTimeGroupItem.Day);

            // Создать ещё один DateTimeGroupItem, сгруппированный по дню, чтобы продемонстрировать важность свойства Day
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

### См. также

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


