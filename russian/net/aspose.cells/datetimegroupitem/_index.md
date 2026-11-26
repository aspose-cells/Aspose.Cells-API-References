---
title: "Класс DateTimeGroupItem"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.DateTimeGroupItem. Представляет настройку группировки даты и времени"
type: docs
url: /ru/net/aspose.cells/datetimegroupitem/
---
## DateTimeGroupItem class

Представляет настройку группировки по дате и времени.

```csharp
public class DateTimeGroupItem
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [DateTimeGroupItem](datetimegroupitem/)(DateTimeGroupingType, int, int, int, int, int, int) |  |

## Свойства

| Имя | Описание |
| --- | --- |
| [DateTimeGroupingType](../../aspose.cells/datetimegroupitem/datetimegroupingtype/) { get; set; } | Получает и задаёт тип группы. |
| [Day](../../aspose.cells/datetimegroupitem/day/) { get; set; } | Получает и задаёт день сгруппированной даты и времени. |
| [Hour](../../aspose.cells/datetimegroupitem/hour/) { get; set; } | Получает и задаёт час сгруппированной даты и времени. |
| [Minute](../../aspose.cells/datetimegroupitem/minute/) { get; set; } | Получает и задаёт минуту сгруппированной даты и времени. |
| [MinValue](../../aspose.cells/datetimegroupitem/minvalue/) { get; } | Получает минимальное значение. |
| [Month](../../aspose.cells/datetimegroupitem/month/) { get; set; } | Получает и задаёт месяц сгруппированной даты и времени. |
| [Second](../../aspose.cells/datetimegroupitem/second/) { get; set; } | Получает и задаёт секунду сгруппированной даты и времени. |
| [Year](../../aspose.cells/datetimegroupitem/year/) { get; set; } | Получает и задаёт год сгруппированной даты и времени. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupItemDemo
    {
        public static void DateTimeGroupItemExample()
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

            // Доступ к свойствам
            Console.WriteLine("MinValue: " + dateTimeGroupItem.MinValue);
            Console.WriteLine("DateTimeGroupingType: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Year: " + dateTimeGroupItem.Year);
            Console.WriteLine("Month: " + dateTimeGroupItem.Month);
            Console.WriteLine("Day: " + dateTimeGroupItem.Day);
            Console.WriteLine("Hour: " + dateTimeGroupItem.Hour);
            Console.WriteLine("Minute: " + dateTimeGroupItem.Minute);
            Console.WriteLine("Second: " + dateTimeGroupItem.Second);

            // Изменение свойств
            dateTimeGroupItem.DateTimeGroupingType = DateTimeGroupingType.Month;
            dateTimeGroupItem.Year = 2022;
            dateTimeGroupItem.Month = 12;
            dateTimeGroupItem.Day = 25;
            dateTimeGroupItem.Hour = 10;
            dateTimeGroupItem.Minute = 15;
            dateTimeGroupItem.Second = 30;

            // Доступ к изменённым свойствам
            Console.WriteLine("Modified DateTimeGroupingType: " + dateTimeGroupItem.DateTimeGroupingType);
            Console.WriteLine("Modified Year: " + dateTimeGroupItem.Year);
            Console.WriteLine("Modified Month: " + dateTimeGroupItem.Month);
            Console.WriteLine("Modified Day: " + dateTimeGroupItem.Day);
            Console.WriteLine("Modified Hour: " + dateTimeGroupItem.Hour);
            Console.WriteLine("Modified Minute: " + dateTimeGroupItem.Minute);
            Console.WriteLine("Modified Second: " + dateTimeGroupItem.Second);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


