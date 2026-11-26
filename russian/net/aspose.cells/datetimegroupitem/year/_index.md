---
title: "DateTimeGroupItem.Year"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DateTimeGroupItem. Получает и задаёт год сгруппированной даты и времени"
type: docs
url: /ru/net/aspose.cells/datetimegroupitem/year/
---
## DateTimeGroupItem.Year property

Получает и задаёт год сгруппированной даты и времени.

```csharp
public int Year { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DateTimeGroupItemPropertyYearDemo
    {
        public static void Run()
        {
            // Создать DateTimeGroupItem, сгруппированный по году
            DateTimeGroupItem dateTimeGroup = new DateTimeGroupItem(
                DateTimeGroupingType.Year,
                2023,  // Year
                1,     // Month (ignored when grouping by Year)
                1,     // Day (ignored)
                0,     // Hour (ignored)
                0,     // Minute (ignored)
                0      // Second (ignored)
            );

            // Отобразить начальное значение Year
            Console.WriteLine("Initial Year: " + dateTimeGroup.Year);

            // Изменить свойство Year
            dateTimeGroup.Year = 2024;

            // Отобразить изменённое значение Year
            Console.WriteLine("Modified Year: " + dateTimeGroup.Year);

            // Показать, что другие свойства игнорируются при группировке по Year
            dateTimeGroup.Month = 12;
            Console.WriteLine("Month value is ignored when grouping by Year: " + dateTimeGroup.Month);
        }
    }
}
```

### См. также

* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


