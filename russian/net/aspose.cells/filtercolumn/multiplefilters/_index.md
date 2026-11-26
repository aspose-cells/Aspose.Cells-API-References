---
title: "FilterColumn.MultipleFilters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FilterColumn. Получает MultipleFilterCollection для фильтрации данных по меткам или дате и времени"
type: docs
url: /ru/net/aspose.cells/filtercolumn/multiplefilters/
---
## FilterColumn.MultipleFilters property

Получает [`MultipleFilterCollection`](../../multiplefiltercollection/) для фильтрации данных по меткам или дате и времени.

```csharp
[Obsolete("Use FilterColumn.FilterValues instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MultipleFilterCollection MultipleFilters { get; set; }
```

### Примечания

NOTE: Этот член теперь устарел. Вместо него, пожалуйста, используйте свойство FilterColumn.FilterValues. Это свойство будет удалено через 12 месяцев, начиная с июня 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyMultipleFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Добавьте примерные данные
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("Fruit");
                worksheet.Cells["A3"].PutValue("Vegetable");
                worksheet.Cells["A4"].PutValue("Fruit");
                worksheet.Cells["A5"].PutValue("Grain");

                // Применить автофильтр к диапазону
                worksheet.AutoFilter.Range = "A1:A5";

                // Получить первый столбец фильтра
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // Создать и установить MultipleFilters
                MultipleFilterCollection multipleFilters = new MultipleFilterCollection();
                multipleFilters.Add("Fruit");
                multipleFilters.Add("Vegetable");
                multipleFilters.MatchBlank = false;

                // Назначить MultipleFilters столбцу фильтра
                filterColumn.MultipleFilters = multipleFilters;

                // Отобразить свойства MultipleFilters
                Console.WriteLine("MultipleFilters Count: " + filterColumn.MultipleFilters.Count);
                Console.WriteLine("MatchBlank: " + filterColumn.MultipleFilters.MatchBlank);

                // Сохраните книгу
                workbook.Save("MultipleFiltersDemo.xlsx");
                Console.WriteLine("MultipleFilters demonstration completed successfully.");
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

* class [MultipleFilterCollection](../../multiplefiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


