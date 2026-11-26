---
title: "Класс CustomFilter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.CustomFilter. Представляет пользовательский фильтр"
type: docs
url: /ru/net/aspose.cells/customfilter/
---
## CustomFilter class

Представляет пользовательский фильтр.

```csharp
public class CustomFilter
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Criteria](../../aspose.cells/customfilter/criteria/) { get; set; } | Получает и задает критерий. |
| [FilterOperatorType](../../aspose.cells/customfilter/filteroperatortype/) { get; set; } | Получает и задает тип оператора фильтра. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetCriteria](../../aspose.cells/customfilter/setcriteria/)(FilterOperatorType, object) | Задает критерий фильтра. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCustomFilterDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Добавить примерные данные в лист
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["A5"].PutValue(40);

                // Применить автофильтр к диапазону
                worksheet.AutoFilter.Range = "A1:A5";
                AutoFilter filter = worksheet.AutoFilter;

                // Применить пользовательский фильтр, чтобы получить экземпляр CustomFilter
                filter.Custom(0, FilterOperatorType.GreaterThan, 25);

                // Получить первый пользовательский фильтр из коллекции фильтров
                CustomFilter customFilter = ((CustomFilterCollection)filter.FilterColumns[0].Filter)[0];

                // Отобразить свойства фильтра
                Console.WriteLine("Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Criteria Value: " + customFilter.Criteria);

                // Изменить критерий фильтра с помощью метода SetCriteria
                customFilter.SetCriteria(FilterOperatorType.LessThan, 35);

                // Отобразить обновленные свойства фильтра
                Console.WriteLine("Updated Filter Operator: " + customFilter.FilterOperatorType);
                Console.WriteLine("Updated Criteria Value: " + customFilter.Criteria);

                // Сохраните книгу
                workbook.Save("CustomFilterDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CustomFilter: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


