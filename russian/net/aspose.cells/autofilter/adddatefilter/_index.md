---
title: "AutoFilter.AddDateFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод AutoFilter. Добавляет фильтр по дате"
type: docs
url: /ru/net/aspose.cells/autofilter/adddatefilter/
---
## AutoFilter.AddDateFilter method

Добавляет фильтр по дате.

```csharp
public void AddDateFilter(int fieldIndex, DateTimeGroupingType dateTimeGroupingType, int year, 
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
    public class AutoFilterMethodAddDateFilterWithInt32DateTimeGroupingTypeInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1, 10, 0, 0));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 1, 1, 11, 0, 0));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 1, 2, 10, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 2, 1, 10, 0, 0));

            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:A5";

            autoFilter.AddDateFilter(0, DateTimeGroupingType.Month, 2023, 1, 1, 0, 0, 0);
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Day, 2023, 1, 2, 0, 0, 0);

            workbook.Save("AutoFilterAddDateFilterExample.xlsx");
        }
    }
}
```

### См. также

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


