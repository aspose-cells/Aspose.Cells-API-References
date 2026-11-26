---
title: "PivotDateTimeRangeGroupSettings.Interval"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotDateTimeRangeGroupSettings. Возвращает внутреннее значение группы"
type: docs
url: /ru/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/
---
## PivotDateTimeRangeGroupSettings.Interval property

Получает внутреннее значение группы.

```csharp
public double Interval { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDateTimeRangeGroupSettingsPropertyIntervalDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Добавить лист с образцовыми данными
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Добавить примерные данные даты
            dataSheet.Cells["A1"].PutValue("Date");
            dataSheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-5));
            dataSheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-4));
            dataSheet.Cells["A4"].PutValue(DateTime.Now.AddDays(-3));
            dataSheet.Cells["A5"].PutValue(DateTime.Now.AddDays(-2));
            dataSheet.Cells["A6"].PutValue(DateTime.Now.AddDays(-1));
            dataSheet.Cells["A7"].PutValue(DateTime.Now);

            // Добавить лист с сводной таблицей
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            
            // Добавьте сводную таблицу
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:A7", 
                "A1", 
                "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // Добавьте поле даты в область строк
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField dateField = pivotTable.RowFields[0];

            // Группировать по дням с интервалом 2
            dateField.GroupBy(1, false);
            PivotDateTimeRangeGroupSettings groupSettings = 
                (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            
            // Поскольку Interval доступен только для чтения, его необходимо установить во время группировки
            // Интервал фактически задаётся в параметрах метода GroupBy
            // Здесь мы просто проверяем значение интервала
            Console.WriteLine($"Grouping interval: {groupSettings.Interval} days");

            // Сохраните книгу
            workbook.Save("PivotDateTimeGroupingDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


