---
title: "WebQueryConnection.Url"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebQueryConnection. URL, используемый для обновления внешних данных"
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/url/
---
## WebQueryConnection.Url property

URL, используемый для обновления внешних данных.

```csharp
public string Url { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyUrlDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте подключение веб‑запроса, добавив его в коллекцию
            // Коллекция, вероятно, создаст и вернёт объект подключения
            WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];

            // Установите начальный URL для веб‑запроса
            connection.Url = "https://example.com/data.html";
            Console.WriteLine("Initial URL: " + connection.Url);

            // Измените URL на другой источник
            connection.Url = "https://example.com/updated-data.xml";
            Console.WriteLine("Updated URL: " + connection.Url);

            // Настройте подключение для разбора XML‑данных
            connection.IsXml = true;

            // Обновите соединение данных (обычно это извлекает данные по URL)
            // Примечание: Для реального доступа к вебу требуется сетевое подключение
            // workbook.RefreshAllConnections();

            // Сохраните книгу с подключением веб‑запроса
            workbook.Save("WebQueryConnectionUrlDemo.xlsx");
        }
    }
}
```

### См. также

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


