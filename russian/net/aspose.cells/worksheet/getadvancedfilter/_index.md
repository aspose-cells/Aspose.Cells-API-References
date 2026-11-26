---
title: "Worksheet.GetAdvancedFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Получает настройки расширенного фильтра"
type: docs
url: /ru/net/aspose.cells/worksheet/getadvancedfilter/
---
## Worksheet.GetAdvancedFilter method

Получает настройки расширенного фильтра.

```csharp
public AdvancedFilter GetAdvancedFilter()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetAdvancedFilterDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Настроить данные для фильтрации
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Alice");
            sheet.Cells["A4"].PutValue("Bob");
            
            // Настроить диапазон критериев
            sheet.Cells["C1"].PutValue("Name");
            sheet.Cells["C2"].PutValue("John");
            
            // Применить расширенный фильтр
            sheet.AdvancedFilter(true, "A1:A4", "C1:C2", "E1", false);
            
            // Получить расширенный фильтр
            AdvancedFilter filter = sheet.GetAdvancedFilter();
            
            // Вывести диапазоны фильтра
            Console.WriteLine("List Range: " + filter.ListRange);
            Console.WriteLine("Criteria Range: " + filter.CriteriaRange);
            Console.WriteLine("Copy To Range: " + filter.CopyToRange);
        }
    }
}
```

### См. также

* class [AdvancedFilter](../../advancedfilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


