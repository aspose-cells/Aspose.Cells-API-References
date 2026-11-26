---
title: "QueryTable.ConnectionId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство QueryTable. Возвращает идентификатор соединения таблицы запросов"
type: docs
url: /ru/net/aspose.cells/querytable/connectionid/
---
## QueryTable.ConnectionId property

Получает идентификатор соединения query table.

```csharp
public int ConnectionId { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyConnectionIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для имитации сценария таблицы запросов
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Sample Data");

            try
            {
                // Проверить, есть ли какие‑либо query tables в листе
                if (worksheet.QueryTables.Count > 0)
                {
                    // Получить первую query table
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Отобразить значение свойства ConnectionId (только для чтения)
                    Console.WriteLine("Query Table ConnectionId: " + queryTable.ConnectionId);

                    // Отобразить другие связанные свойства для контекста
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("External Connection: " +
                        (queryTable.ExternalConnection != null ? queryTable.ExternalConnection.Name : "None"));
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Сохраните книгу
                workbook.Save("ConnectionIdDemo.xlsx");
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


