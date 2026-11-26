---
title: "CustomFilter.FilterOperatorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CustomFilter. Получает и задаёт тип оператора фильтра"
type: docs
url: /ru/net/aspose.cells/customfilter/filteroperatortype/
---
## CustomFilter.FilterOperatorType property

Получает и задает тип оператора фильтра.

```csharp
public FilterOperatorType FilterOperatorType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomFilterPropertyFilterOperatorTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Names");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Mike");
            worksheet.Cells["A5"].PutValue("Emily");

            // Применить автофильтр
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Применить пользовательский фильтр с оператором Contains
            filter.Custom(0, FilterOperatorType.Contains, "e");
            
            // Получить первый пользовательский фильтр
            CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];
            
            // Продемонстрировать свойство FilterOperatorType
            Console.WriteLine("Initial Filter Operator: " + customFilter.FilterOperatorType);
            Console.WriteLine("Criteria: " + customFilter.Criteria);
            
            // Изменить тип оператора фильтра
            customFilter.FilterOperatorType = FilterOperatorType.EndsWith;
            Console.WriteLine("Updated Filter Operator: " + customFilter.FilterOperatorType);
            
            // Сохраните книгу
            workbook.Save("FilterOperatorTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


