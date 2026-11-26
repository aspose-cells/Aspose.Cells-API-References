---
title: "Класс PivotDateTimeRangeGroupSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Pivot.PivotDateTimeRangeGroupSettings. Представляет поле, сгруппированное по диапазону даты и времени"
type: docs
url: /ru/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/
---
## PivotDateTimeRangeGroupSettings class

Представляет поле, сгруппированное по диапазону даты и времени.

```csharp
public class PivotDateTimeRangeGroupSettings : PivotFieldGroupSettings
```

## Свойства

| Имя | Описание |
| --- | --- |
| [End](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/end/) { get; } | Получает конечную дату и время группы. |
| [GroupByTypes](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/groupbytypes/) { get; } | Получает типы группировки по дате и времени. |
| [Interval](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/) { get; } | Получает внутреннее значение группы. |
| [Start](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/start/) { get; } | Получает начальную дату и время группы. |
| override [Type](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/type/) { get; } | Получает тип группировки по времени данных. |

## Методы

| Имя | Описание |
| --- | --- |
| [IsGroupedBy](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/isgroupedby/)(PivotGroupByType) | Проверьте, сгруппировано ли поле по типу. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotDateTimeRangeGroupSettingsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавить примерные данные с датами
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
                worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
                worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["B4"].PutValue(30);

                // Создать сводную таблицу
                int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // Добавить поля в сводную таблицу
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

                // Группировать поле даты по месяцам
                PivotField dateField = pivotTable.RowFields[0];
                DateTime startDate = new DateTime(2023, 1, 1);
                DateTime endDate = new DateTime(2023, 12, 31);
                dateField.GroupBy(startDate, endDate, new PivotGroupByType[] { PivotGroupByType.Months }, 1, false);

                // Получить настройки группы
                PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

                // Отобразить свойства настроек группы
                Console.WriteLine($"Group Type: {groupSettings.Type}");
                Console.WriteLine($"Start Date: {groupSettings.Start}");
                Console.WriteLine($"End Date: {groupSettings.End}");
                Console.WriteLine($"Interval: {groupSettings.Interval}");
                Console.WriteLine($"Group By Types: {string.Join(", ", groupSettings.GroupByTypes)}");

                // Проверить, сгруппировано ли по месяцам
                bool isGroupedByMonths = groupSettings.IsGroupedBy(PivotGroupByType.Months);
                Console.WriteLine($"Is grouped by months: {isGroupedByMonths}");

                // Сохраните книгу
                workbook.Save("PivotDateTimeRangeGroupSettingsDemo.xlsx");
                Console.WriteLine("PivotDateTimeRangeGroupSettings demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in PivotDateTimeRangeGroupSettings demo: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PivotFieldGroupSettings](../pivotfieldgroupsettings/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


