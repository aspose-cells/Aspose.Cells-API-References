---
title: "Перечисление TimePeriodType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.TimePeriodType. Используется в правиле условного форматирования FormatConditionType.TimePeriod. Это динамические периоды времени, которые меняются в зависимости от даты обновления/применения условного форматирования."
type: docs
url: /ru/net/aspose.cells/timeperiodtype/
---
## TimePeriodType enumeration

Используется в правиле условного форматирования FormatConditionType.TimePeriod. Это динамические временные периоды, которые меняются в зависимости от даты обновления/применения условного форматирования.

```csharp
public enum TimePeriodType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Today | `0` | Текущая дата. |
| Yesterday | `1` | Вчерашняя дата. |
| Tomorrow | `2` | Завтрашняя дата. |
| Last7Days | `3` | Дата за последние семь дней. |
| ThisMonth | `4` | Дата, происходящая в текущем календарном месяце. |
| LastMonth | `5` | Дата, произошедшая в прошлом календарном месяце. |
| NextMonth | `6` | Дата, произошедшая в следующем календарном месяце. |
| ThisWeek | `7` | Дата, произошедшая на этой неделе. |
| LastWeek | `8` | Дата, произошедшая на прошлой неделе. |
| NextWeek | `9` | Дата, произошедшая на следующей неделе. |
| ThisYear | `10` | Дата, произошедшая в этом году. Только для .ods. |
| LastYear | `11` | Дата, произошедшая в прошлом году. Только для .ods. |
| NextYear | `12` | Дата, произошедшая в следующем году. Только для .ods. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TimePeriodTypeDemo
    {
        public static void TimePeriodTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить правило условного форматирования
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Определить область ячеек для условного форматирования
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Добавить условие для периода времени
            int conditionIndex = fcs.AddCondition(FormatConditionType.TimePeriod);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.LightBlue;

            // Установить тип периода времени
            fc.TimePeriod = TimePeriodType.Today;

            // Сохраните книгу
            workbook.Save("TimePeriodTypeExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


