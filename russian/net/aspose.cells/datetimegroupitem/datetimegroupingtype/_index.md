---
title: "DateTimeGroupItem.DateTimeGroupingType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DateTimeGroupItem. Получает и задает тип группы"
type: docs
url: /ru/net/aspose.cells/datetimegroupitem/datetimegroupingtype/
---
## DateTimeGroupItem.DateTimeGroupingType property

Получает и задаёт тип группы.

```csharp
public DateTimeGroupingType DateTimeGroupingType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyDateTimeGroupingTypeDemo
    {
        public static void Run()
        {
            // Создайте экземпляр DateTimeGroupItem
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year, // Group by Year
                2023,                      // Year
                10,                       // Month
                5,                         // Day
                14,                       // Hour
                30,                       // Minute
                45                        // Second
            );

            // Отобразить начальные свойства
            Console.WriteLine("Initial Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine($"Date Components: {dateTimeGroupItem.Year}-{dateTimeGroupItem.Month}-{dateTimeGroupItem.Day}");

            // Изменить тип группировки и компоненты даты
            dateTimeGroupItem.DateTimeGroupingType = DateTimeGroupingType.Month;
            dateTimeGroupItem.Year = 2022;
            dateTimeGroupItem.Month = 12;

            // Отобразить изменённые свойства
            Console.WriteLine("Modified Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine($"Modified Date Components: {dateTimeGroupItem.Year}-{dateTimeGroupItem.Month}");
        }
    }
}
```

### См. также

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


