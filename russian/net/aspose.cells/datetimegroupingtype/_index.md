---
title: "Перечисление DateTimeGroupingType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.DateTimeGroupingType. Указывает, как группировать значения DateTime"
type: docs
url: /ru/net/aspose.cells/datetimegroupingtype/
---
## DateTimeGroupingType enumeration

Указывает, как группировать значения даты и времени.

```csharp
public enum DateTimeGroupingType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Day | `0` | Группировать по дню. |
| Hour | `1` | Группировать по часу. |
| Minute | `2` | Группировать по минуте. |
| Month | `3` | Группировать по месяцу. |
| Second | `4` | Группировать по секунде. |
| Year | `5` | Группировать по году. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupingTypeDemo
    {
        public static void DateTimeGroupingTypeExample()
        {
            // Создание книги и доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавление некоторых образцовых данных
            worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1, 10, 0, 0));
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1, 11, 0, 0));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 1, 2, 10, 0, 0));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 1, 2, 11, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 2, 1, 10, 0, 0));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 2, 1, 11, 0, 0));

            // Создание AutoFilter и установка диапазона
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.Range = "A1:A6";

            // Добавление фильтров даты с различным DateTimeGroupingType
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Month, 2023, 1, 1, 0, 0, 0);
            autoFilter.AddDateFilter(0, DateTimeGroupingType.Hour, 2023, 1, 1, 10, 0, 0);
            
            // Сохранение книги
            workbook.Save("DateTimeGroupingTypeExample.xlsx");
            workbook.Save("DateTimeGroupingTypeExample.pdf");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


