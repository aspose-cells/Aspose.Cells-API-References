---
title: "DateTimeGroupItem.Month"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DateTimeGroupItem. Получает и задает месяц сгруппированного даты и времени"
type: docs
url: /ru/net/aspose.cells/datetimegroupitem/month/
---
## DateTimeGroupItem.Month property

Получает и задаёт месяц сгруппированной даты и времени.

```csharp
public int Month { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyMonthDemo
    {
        public static void Run()
        {
            // Создать DateTimeGroupItem, сгруппированный по месяцу
            DateTimeGroupItem dateTimeGroupItem = new DateTimeGroupItem(
                DateTimeGroupingType.Month,
                2023,
                10,
                1,
                0,
                0,
                0
            );

            // Отобразить начальное значение месяца
            Console.WriteLine("Initial Month: " + dateTimeGroupItem.Month);

            // Изменить значение месяца
            dateTimeGroupItem.Month = 12;
            Console.WriteLine("Modified Month: " + dateTimeGroupItem.Month);

            // Создать ещё один DateTimeGroupItem с другой группировкой
            DateTimeGroupItem yearlyItem = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,
                1,
                1,
                0,
                0,
                0
            );

            // Показать, что свойство Month всё ещё доступно, даже когда сгруппировано по Year
            Console.WriteLine("Yearly Grouping - Month: " + yearlyItem.Month);
        }
    }
}
```

### См. также

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


