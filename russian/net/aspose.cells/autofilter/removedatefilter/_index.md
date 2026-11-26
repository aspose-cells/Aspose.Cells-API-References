---
title: "AutoFilter.RemoveDateFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AutoFilter. Удаляет фильтр по дате"
type: docs
url: /ru/net/aspose.cells/autofilter/removedatefilter/
---
## AutoFilter.RemoveDateFilter method

Удаляет фильтр по дате.

```csharp
public void RemoveDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
    int month, int day, int hour, int minute, int second)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldIndex | Int32 | Целочисленное смещение поля, на основе которого вы хотите построить фильтр (от левого края списка; самое левое поле имеет индекс 0). |
| dateTimeGroupingType | DateTimeGroupingType | Тип группировки |
| год | Int32 | Год. |
| месяц | Int32 | Месяц. |
| день | Int32 | День. |
| час | Int32 | Час. |
| минута | Int32 | Минута. |
| секунда | Int32 | Секунда. |

### Примечания

Если DateTimeGroupingType равен Year, влияет только параметр year. Если DateTiemGroupingType равен Month, влияют только параметры year и month.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodRemoveDateFilterWithInt32DateTimeGroupingTypeInt32Demo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Добавить примерные данные с датами
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue(new DateTime(2020, 1, 7));
            sheet.Cells["A3"].PutValue(new DateTime(2020, 1, 8));
            sheet.Cells["A4"].PutValue(new DateTime(2020, 1, 9));
            
            // Применить автофильтр
            sheet.AutoFilter.Range = "A1:A4";
            
            // Добавить фильтр даты для дня 7
            sheet.AutoFilter.AddDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            sheet.AutoFilter.Refresh();
            
            // Проверить, что фильтр применён
            Console.WriteLine("Row 2 hidden: " + sheet.Cells.IsRowHidden(1)); // Should be true
            
            // Удалить фильтр даты
            sheet.AutoFilter.RemoveDateFilter(0, DateTimeGroupingType.Day, 2020, 1, 7, 0, 0, 0);
            sheet.AutoFilter.Refresh();
            
            // Проверить, что фильтр удалён
            Console.WriteLine("Row 2 hidden after removal: " + sheet.Cells.IsRowHidden(1)); // Should be false
        }
    }
}
```

### См. также

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


