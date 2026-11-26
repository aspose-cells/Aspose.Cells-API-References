---
title: "FilterColumnCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FilterColumnCollection. Получает объект FilterColumn в специальном поле"
type: docs
url: /ru/net/aspose.cells/filtercolumncollection/item/
---
## FilterColumnCollection indexer

Получает объект [`FilterColumn`](../../filtercolumn/) в специальном поле.

```csharp
public FilterColumn this[int fieldIndex] { get; }
```

| Параметр | Описание |
| --- | --- |
| fieldIndex | Целочисленное смещение поля, на основе которого вы хотите построить фильтр (от левого края списка; самое левое поле имеет индекс 0). |

### Возвращаемое значение

Возвращает объект [`FilterColumn`](../../filtercolumn/).

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");
            sheet.Cells["A5"].PutValue("Date");

            // Применить автофильтр
            sheet.AutoFilter.Range = "A1:A5";
            sheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "e");

            // Доступ к фильтру с помощью свойства Item
            AutoFilter filter = sheet.AutoFilter;
            FilterColumn filterColumn = filter.FilterColumns[0]; // Using Item property
            CustomFilterCollection customFilters = (CustomFilterCollection)filterColumn.Filter;
            CustomFilter firstFilter = customFilters[0];

            // Отобразить свойства фильтра
            Console.WriteLine("Filter Operator Type: " + firstFilter.FilterOperatorType);
            Console.WriteLine("Filter Criteria: " + firstFilter.Criteria);

            // Изменить фильтр
            firstFilter.FilterOperatorType = FilterOperatorType.EndsWith;
            Console.WriteLine("\nModified Filter Operator Type: " + firstFilter.FilterOperatorType);

            // Сохраните книгу
            wb.Save("FilterExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [FilterColumn](../../filtercolumn/)
* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


