---
title: "CustomFilter.SetCriteria"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CustomFilter. Устанавливает критерий фильтра"
type: docs
url: /ru/net/aspose.cells/customfilter/setcriteria/
---
## CustomFilter.SetCriteria method

Задает критерий фильтра.

```csharp
public void SetCriteria(FilterOperatorType filterOperator, object criteria)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filterOperator | FilterOperatorType | тип оператора фильтра |
| критерий | Object | значение критерия фильтра |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterMethodSetCriteriaWithFilterOperatorTObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);

            // Применить автофильтр
            worksheet.AutoFilter.Range = "A1:A5";
            AutoFilter filter = worksheet.AutoFilter;

            try
            {
                // Применить пользовательский фильтр, чтобы получить экземпляр CustomFilter
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // Получить первый пользовательский фильтр из коллекции фильтров
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // Установить критерий с помощью метода SetCriteria
                customFilter.SetCriteria(FilterOperatorType.GreaterThan, 25);

                // Отобразить установленный критерий
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // Сохраните книгу
                workbook.Save("SetCriteriaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* enum [FilterOperatorType](../../filteroperatortype/)
* class [CustomFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


