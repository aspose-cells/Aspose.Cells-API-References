---
title: "Перечисление PivotGroupByType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Pivot.PivotGroupByType. Представляет тип группировки."
type: docs
url: /ru/net/aspose.cells.pivot/pivotgroupbytype/
---
## PivotGroupByType enumeration

Представляет тип группировки.

```csharp
[Flags]
public enum PivotGroupByType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| RangeOfValues | `1` | Группировка по числам. |
| Numbers | `1` | Группировка по числам. |
| Seconds | `2` | Представляет тип группировки по секундам. |
| Minutes | `4` | Представляет тип группировки по минутам. |
| Hours | `8` | Представляет тип группировки по часам. |
| Days | `10` | Представляет тип группировки по дням. |
| Months | `20` | Представляет тип группировки по месяцам. |
| Quarters | `40` | Представляет тип группировки по кварталам. |
| Years | `80` | Представляет тип группировки по годам. |
| DateTimes | `FE` | Представляет все типы группировки дат и времени. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotGroupByTypeDemo
    {
        public static void PivotGroupByTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Date");
            Style style = workbook.CreateStyle();
            style.Number = 14;//m/d/yyy
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A2"].SetStyle(style);

            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A3"].SetStyle(style);

            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A4"].SetStyle(style);

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавьте поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value field

            //TODO
            PivotField dateField = pivotTable.RowFields[0];

            DateTime start = new DateTime(2023, 1, 1);
            DateTime end = new DateTime(2023, 12, 31);
            dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, false);

            // Доступ к настройкам группировки
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

            // Вывод настроек группировки
            Console.WriteLine("Group Type: " + groupSettings.Type);
            Console.WriteLine("Start Date: " + groupSettings.Start);
            Console.WriteLine("End Date: " + groupSettings.End);
            Console.WriteLine("Interval: " + groupSettings.Interval);
            Console.WriteLine("Is Grouped By Months: " + groupSettings.IsGroupedBy(PivotGroupByType.Months));

            // Сохраните книгу
            workbook.Save("PivotGroupByTypeExample.xlsx");
            
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


