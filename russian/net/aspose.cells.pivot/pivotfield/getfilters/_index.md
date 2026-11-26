---
title: "PivotField.GetFilters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotField. Получает все фильтры сводки, применённые к этому полю"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/getfilters/
---
## PivotField.GetFilters method

Получает все фильтры сводки, применённые к этому полю сводки.

```csharp
public PivotFilter[] GetFilters()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGetFiltersDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["B1"].Value = "Sales";
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].Value = DateTime.Now.AddDays(i-2);
                worksheet.Cells[$"B{i}"].Value = i * 100;
            }

            // Создать сводную таблицу
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B10", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Добавить поле строки и поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Применить фильтр даты
            PivotField dateField = pivotTable.RowFields[0];
            DateTime startDate = DateTime.Now;
            DateTime endDate = DateTime.Now.AddDays(5);
            dateField.FilterByDate(PivotFilterType.DateBetween, startDate, endDate);
            
            // Получить и отобразить фильтры
            PivotFilter[] filters = dateField.GetFilters();
            Console.WriteLine($"Number of filters applied: {filters.Length}");
            if (filters.Length > 0)
            {
                Console.WriteLine($"Filter type: {filters[0].FilterType}");
                Console.WriteLine($"Start date: {filters[0].GetDateTimeValues()[0]}");
                Console.WriteLine($"End date: {filters[0].GetDateTimeValues()[1]}");
            }
            
            // Сохраните книгу
            workbook.Save("PivotFieldGetFiltersDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotFilter](../../pivotfilter/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


