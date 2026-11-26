---
title: "Перечисление PivotFieldGroupType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Pivot.PivotFieldGroupType. Представляет тип группы поля сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfieldgrouptype/
---
## PivotFieldGroupType enumeration

Представляет тип группировки поля сводной таблицы.

```csharp
public enum PivotFieldGroupType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Нет группы |
| DateTimeRange | `1` | Сгруппировано по диапазону DateTime. |
| NumbericRange | `2` | Сгруппировано по числовому диапазону. |
| NumericRange | `2` | Сгруппировано по числовому диапазону. |
| Discrete | `3` | Сгруппировано по дискретным точкам. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotFieldGroupTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Добавить новый лист в книгу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Date");
            Style style = workbook.CreateStyle();
            style.Number = 14; // m/d/yyyy format
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

            // Сгруппировать поле даты
            PivotField dateField = pivotTable.RowFields[0];
            DateTime start = new DateTime(2023, 1, 1);
            DateTime end = new DateTime(2023, 12, 31);
            dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, false);

            // Получить доступ и отобразить настройки группы
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            Console.WriteLine("Group Type: " + groupSettings.Type);
            Console.WriteLine("Interval: " + groupSettings.Interval);
            Console.WriteLine("Is Grouped By Months: " + groupSettings.IsGroupedBy(PivotGroupByType.Months));

            // Сохраните книгу
            workbook.Save("PivotFieldGroupTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


