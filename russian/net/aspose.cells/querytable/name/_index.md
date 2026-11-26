---
title: "QueryTable.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство QueryTable. Возвращает имя таблицы запросов"
type: docs
url: /ru/net/aspose.cells/querytable/name/
---
## QueryTable.Name property

Получает имя querytable.

```csharp
public string Name { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для симуляции таблицы запросов
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            try
            {
                // Проверить, есть ли какие‑либо query tables в листе
                if (worksheet.QueryTables.Count > 0)
                {
                    // Получить первую query table
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Отобразить значение свойства Name (операция только для чтения)
                    Console.WriteLine("Query Table Name: " + queryTable.Name);

                    // Отобразить другие свойства только для чтения для контекста
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                    Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Сохраните книгу
                workbook.Save("QueryTableNameDemo.xlsx");
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

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


