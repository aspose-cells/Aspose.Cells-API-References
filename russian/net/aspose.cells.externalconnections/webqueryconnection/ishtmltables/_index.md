---
title: "WebQueryConnection.IsHtmlTables"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebQueryConnection. Флаг, указывающий, должны ли веб‑запросы работать только с HTML‑таблицами"
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/ishtmltables/
---
## WebQueryConnection.IsHtmlTables property

Флаг, указывающий, должны ли веб‑запросы работать только с HTML‑таблицами.

```csharp
public bool IsHtmlTables { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsHtmlTablesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();

            try
            {
                // Создайте подключение веб‑запроса через индексатор коллекции
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];

                Console.WriteLine("Initial IsHtmlTables: " + connection.IsHtmlTables);
                
                connection.IsHtmlTables = true;
                Console.WriteLine("Updated IsHtmlTables: " + connection.IsHtmlTables);

                workbook.Save("IsHtmlTablesDemo.xlsx");
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

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


