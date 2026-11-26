---
title: "DateTimeGroupItem.Hour"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DateTimeGroupItem. Получает и задает час сгруппированного даты и времени"
type: docs
url: /ru/net/aspose.cells/datetimegroupitem/hour/
---
## DateTimeGroupItem.Hour property

Получает и задаёт час сгруппированной даты и времени.

```csharp
public int Hour { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyHourDemo
    {
        public static void Run()
        {
            // Создать DateTimeGroupItem с группировкой по часам
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Hour,
                2023,  // Year
                10,     // Month
                5,      // Day
                14,     // Hour
                0,      // Minute
                0      // Second
            );

            // Отобразить начальное значение часа
            Console.WriteLine("Initial Hour: " + dateTimeGroupItem.Hour);

            // Изменить свойство hour
            dateTimeGroupItem.Hour = 18;

            // Отобразить изменённое значение hour
            Console.WriteLine("Modified Hour: " + dateTimeGroupItem.Hour);
        }
    }
}
```

### См. также

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


