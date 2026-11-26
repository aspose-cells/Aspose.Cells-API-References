---
title: "FilterColumn.FilterType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FilterColumn. Получает и задает тип данных фильтрации"
type: docs
url: /ru/net/aspose.cells/filtercolumn/filtertype/
---
## FilterColumn.FilterType property

Получает и задает тип фильтрации данных.

```csharp
public FilterType FilterType { get; set; }
```

### Примечания

Соответствующий объект фильтра будет создан, когда это свойство установлено, и соответствующее свойство следует использовать для получения объекта фильтра соответственно:

| **FilterType** | **Property** |
| --- | --- |
| MultipleFilters | [`FilterValues`](../filtervalues/) |
| CustomFilters | [`CustomFilters`](../customfilters/) |
| ColorFilter | [`ColorFilter`](../colorfilter/) |
| DynamicFilter | [`DynamicFilter`](../dynamicfilter/) |
| IconFilter | [`IconFilter`](../iconfilter/) |
| Top10 | [`Top10Filter`](../top10filter/) |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFilterTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Department");
            sheet.Cells["A2"].PutValue("HR");
            sheet.Cells["A3"].PutValue("IT");
            sheet.Cells["A4"].PutValue("Finance");

            sheet.Cells["B1"].PutValue("Employees");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(15);
            sheet.Cells["B4"].PutValue(8);

            // Применить автофильтр, используя строковый диапазон
            sheet.AutoFilter.Range = "A1:B4";

            // Добавить различные типы фильтров для демонстрации свойства FilterType
            sheet.AutoFilter.AddFilter(0, "HR"); // Simple filter
            sheet.AutoFilter.Custom(1, FilterOperatorType.GreaterThan, 10); // Custom filter

            // Получить столбцы фильтра
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // Отобразить FilterType для каждого столбца
            for (int i = 0; i < filterColumns.Count; i++)
            {
                FilterColumn filterColumn = filterColumns[i];
                Console.WriteLine($"Column {i} FilterType: {filterColumn.FilterType}");
            }

            // Сохраните книгу
            workbook.Save("FilterTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [FilterType](../../filtertype/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


