---
title: "CustomFilterCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CustomFilterCollection. Получает пользовательский фильтр по конкретному индексу"
type: docs
url: /ru/net/aspose.cells/customfiltercollection/item/
---
## CustomFilterCollection indexer

Получает пользовательский фильтр по указанному индексу.

```csharp
public CustomFilter this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // Создайте новую CustomFilterCollection
                CustomFilterCollection filters = new CustomFilterCollection();

                // Получите доступ к свойству Item (только для чтения) с помощью индексатора
                // Поскольку коллекция пуста, мы просто продемонстрируем доступ к свойству
                // В реальном сценарии вы сначала добавите фильтры другими способами
                if (filters.Count > 0)
                {
                    CustomFilter firstFilter = filters[0];
                    Console.WriteLine($"First filter operator: {firstFilter.FilterOperatorType}");
                    Console.WriteLine($"First filter criteria: {firstFilter.Criteria}");
                }
                else
                {
                    Console.WriteLine("No filters in collection to demonstrate Item property");
                }

                // Сохраните книгу
                workbook.Save("CustomFilterCollectionItemDemo.xlsx");
                Console.WriteLine("CustomFilterCollection Item property demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating Item property: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [CustomFilter](../../customfilter/)
* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


