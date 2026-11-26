---
title: "AdvancedFilter.CriteriaRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство AdvancedFilter. Возвращает диапазон критериев этого расширенного фильтра"
type: docs
url: /ru/net/aspose.cells/advancedfilter/criteriarange/
---
## AdvancedFilter.CriteriaRange property

Получает диапазон критериев этого расширенного фильтра.

```csharp
public string CriteriaRange { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCriteriaRangeDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Заполните примерными данными диапазон списка
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Food");
            sheet.Cells["B2"].PutValue(120);
            sheet.Cells["A3"].PutValue("Transport");
            sheet.Cells["B3"].PutValue(80);
            sheet.Cells["A4"].PutValue("Food");
            sheet.Cells["B4"].PutValue(150);

            // Заполнить примерные критерии (фильтр будет использовать их при применении)
            sheet.Cells["D1"].PutValue("Category");
            sheet.Cells["D2"].PutValue("Food");

            try
            {
                // Получить объект AdvancedFilter для листа
                AdvancedFilter filter = sheet.GetAdvancedFilter();

                // Свойства ListRange, CriteriaRange и CopyToRange являются только для чтения.
                // Отобразить автоматически определённые диапазоны.
                Console.WriteLine("List Range:    " + filter.ListRange);
                Console.WriteLine("Criteria Range:" + filter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + filter.CopyToRange);

                // Сохранить книгу (необязательно, просто чтобы показать, что файл может быть создан)
                workbook.Save("AdvancedFilterCriteriaRangeDemo.xlsx");
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

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


