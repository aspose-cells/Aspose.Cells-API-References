---
title: "DateTimeGroupItem.Second"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DateTimeGroupItem. Получает и задает секунду сгруппированной даты и времени"
type: docs
url: /ru/net/aspose.cells/datetimegroupitem/second/
---
## DateTimeGroupItem.Second property

Получает и задаёт секунду сгруппированной даты и времени.

```csharp
public int Second { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertySecondDemo
    {
        public static void Run()
        {
            // Создайте экземпляр DateTimeGroupItem
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year, // Group by Year
                2023,                      // Year
                10,                        // Month
                5,                         // Day
                14,                        // Hour
                30,                        // Minute
                45                         // Second
            );

            // Отобразить начальное значение секунды
            Console.WriteLine("Initial Second: " + dateTimeGroupItem.Second);

            // Изменить значение секунды
            dateTimeGroupItem.Second = 50;
            Console.WriteLine("Modified Second: " + dateTimeGroupItem.Second);

            // Создать другой экземпляр с другим значением секунды
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

### См. также

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


