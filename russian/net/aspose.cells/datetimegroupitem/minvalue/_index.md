---
title: "DateTimeGroupItem.MinValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DateTimeGroupItem. Возвращает минимальное значение"
type: docs
url: /ru/net/aspose.cells/datetimegroupitem/minvalue/
---
## DateTimeGroupItem.MinValue property

Получает минимальное значение.

```csharp
public DateTime MinValue { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMinValueDemo
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

            // Продемонстрировать свойство MinValue
            Console.WriteLine("MinValue: " + dateTimeGroupItem.MinValue);

            // Показать другие свойства для контекста
            Console.WriteLine("Grouping Type: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Date Components: {0}-{1}-{2} {3}:{4}:{5}",
                dateTimeGroupItem.Year,
                dateTimeGroupItem.Month,
                dateTimeGroupItem.Day,
                dateTimeGroupItem.Hour,
                dateTimeGroupItem.Minute,
                dateTimeGroupItem.Second);
        }
    }
}
```

### См. также

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


