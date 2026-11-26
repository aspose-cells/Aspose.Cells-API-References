---
title: "FilterColumn.CustomFilters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FilterColumn. Возвращает CustomFilterCollection для фильтрации данных по пользовательским критериям"
type: docs
url: /ru/net/aspose.cells/filtercolumn/customfilters/
---
## FilterColumn.CustomFilters property

Возвращает [`CustomFilterCollection`](../../customfiltercollection/) для фильтрации данных по пользовательским критериям.

```csharp
public CustomFilterCollection CustomFilters { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Сеттер этого свойства теперь устарел. Вместо этого, пожалуйста, используйте свойство [`FilterType`](../filtertype/), задав его как CustomFilters. Это свойство будет удалено через 12 месяцев, начиная с июня 2026 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyCustomFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Добавьте примерные данные
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Cherry");
                worksheet.Cells["A5"].PutValue("Date");
                worksheet.Cells["A6"].PutValue("Elderberry");

                // Применить автофильтр
                worksheet.AutoFilter.Range = "A1:A6";

                // Получите столбец фильтра
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Создайте и задайте пользовательские фильтры с помощью метода AutoFilter.Custom
                // Первый фильтр: начинается с "A"
                worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "A", false, FilterOperatorType.None, null);

                // Второй фильтр: заканчивается на "y" (отношение И)
                worksheet.AutoFilter.Custom(0, FilterOperatorType.EndsWith, "y", true, FilterOperatorType.None, null);

                // Получите пользовательские фильтры из столбца фильтра
                CustomFilterCollection customFilters = filterColumn.CustomFilters;

                // Отобразите информацию о пользовательских фильтрах
                Console.WriteLine($"Number of custom filters: {customFilters.Count}");
                Console.WriteLine($"Filter relationship (And): {customFilters.And}");

                // Примечание: CustomFilterCollection не раскрывает отдельные фильтры напрямую
                // через индексатор, поэтому мы можем только отобразить свойства коллекции
                Console.WriteLine("Custom filters have been applied to the column.");

                // Сохраните книгу
                workbook.Save("CustomFiltersDemo.xlsx");
                Console.WriteLine("CustomFilters demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CustomFilterCollection](../../customfiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


