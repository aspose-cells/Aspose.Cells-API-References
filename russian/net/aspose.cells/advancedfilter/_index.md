---
title: "Класс AdvancedFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.AdvancedFilter. Представляет настройки расширенного фильтра"
type: docs
url: /ru/net/aspose.cells/advancedfilter/
---
## AdvancedFilter class

Представляет настройки расширенного фильтра.

```csharp
public class AdvancedFilter
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CopyToRange](../../aspose.cells/advancedfilter/copytorange/) { get; } | Получает диапазон, в который копируется результат этого расширенного фильтра. |
| [CriteriaRange](../../aspose.cells/advancedfilter/criteriarange/) { get; } | Получает диапазон критериев этого расширенного фильтра. |
| [ListRange](../../aspose.cells/advancedfilter/listrange/) { get; } | Получает диапазон списка этого расширенного фильтра. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAdvancedFilterDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите первый лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Заполните примерными данными диапазон списка
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(1.5);
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["B3"].PutValue(0.8);
                worksheet.Cells["A4"].PutValue("Orange");
                worksheet.Cells["B4"].PutValue(1.2);

                // Заполните диапазон критериев
                worksheet.Cells["D1"].PutValue("Product");
                worksheet.Cells["D2"].PutValue("Apple");

                // Получите экземпляр AdvancedFilter из листа
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // Отобразите свойства только для чтения
                Console.WriteLine("List Range: " + advancedFilter.ListRange);
                Console.WriteLine("Criteria Range: " + advancedFilter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + advancedFilter.CopyToRange);

                // Сохраните книгу
                workbook.Save("AdvancedFilterDemo.xlsx");
                Console.WriteLine("AdvancedFilter demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in AdvancedFilter demonstration: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


