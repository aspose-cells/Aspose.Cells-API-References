---
title: "QueryTable.ExternalConnection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство QueryTable. Возвращает связанное внешнее соединение"
type: docs
url: /ru/net/aspose.cells/querytable/externalconnection/
---
## QueryTable.ExternalConnection property

Получает связанное внешнее соединение.

```csharp
public ExternalConnection ExternalConnection { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class QueryTablePropertyExternalConnectionDemo
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

                    // Получить доступ к свойству ExternalConnection (только для чтения)
                    ExternalConnection externalConnection = queryTable.ExternalConnection;

                    // Отобразить информацию о внешнем соединении
                    if (externalConnection != null)
                    {
                        Console.WriteLine("External Connection ID: " + externalConnection.Id);
                        Console.WriteLine("External Connection Name: " + externalConnection.Name);
                        Console.WriteLine("External Connection Type: " + externalConnection.ClassType);
                        Console.WriteLine("Connection String: " + externalConnection.ConnectionString);
                        Console.WriteLine("Refresh on Load: " + externalConnection.RefreshOnLoad);
                    }
                    else
                    {
                        Console.WriteLine("No external connection associated with this query table.");
                    }

                    // Отобразить другие свойства таблицы запросов для контекста
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Сохраните книгу
                workbook.Save("ExternalConnectionDemo.xlsx");
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

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


