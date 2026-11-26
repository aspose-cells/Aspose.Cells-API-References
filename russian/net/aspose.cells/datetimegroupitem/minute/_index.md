---
title: "DateTimeGroupItem.Minute"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DateTimeGroupItem. Получает и задает минуту сгруппированного даты и времени"
type: docs
url: /ru/net/aspose.cells/datetimegroupitem/minute/
---
## DateTimeGroupItem.Minute property

Получает и задаёт минуту сгруппированной даты и времени.

```csharp
public int Minute { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMinuteDemo
    {
        public static void Run()
        {
            // Создать DateTimeGroupItem с начальными значениями
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,
                10,
                5,
                14,
                30,
                45
            );

            // Отобразить начальное значение минуты
            Console.WriteLine("Initial Minute: " + dateTimeGroupItem.Minute);

            // Изменить значение минуты
            dateTimeGroupItem.Minute = 15;

            // Отобразить изменённое значение минуты
            Console.WriteLine("Modified Minute: " + dateTimeGroupItem.Minute);

            // Создать новый DateTimeGroupItem только с группировкой по минуте
            DateTimeGroupItem minuteGroup = new DateTimeGroupItem(
                DateTimeGroupingType.Minute,
                0, 0, 0, 0, 45, 0
            );

            // Отобразить минуту из группировки по минуте
            Console.WriteLine("Minute from Minute Grouping: " + minuteGroup.Minute);
        }
    }
}
```

### См. также

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


