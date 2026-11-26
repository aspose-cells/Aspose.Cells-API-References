---
title: "WebQueryConnection.Post"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebQueryConnection. Возвращает или задает строку, используемую методом post для ввода данных на веб‑сервер с целью получения данных из веб‑запроса"
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/post/
---
## WebQueryConnection.Post property

Возвращает или задаёт строку, используемую методом POST для ввода данных на веб‑сервер и получения данных из веб‑запроса.

```csharp
public string Post { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyPostDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Создать соединение веб‑запроса, получив доступ к существующему или создав его через правильную инициализацию
                // Поскольку мы не можем напрямую создать экземпляр WebQueryConnection, мы используем первое соединение, если оно существует
                WebQueryConnection connection = null;
                
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection webQueryConn)
                {
                    connection = webQueryConn;
                }
                else
                {
                    // Если соединения не существуют, мы продемонстрируем работу с имитационным соединением
                    Console.WriteLine("No existing web query connection found - demonstrating with property access only");
                    return;
                }
                
                // Установить начальное значение Post
                connection.Post = "param1=value1&param2=value2";
                Console.WriteLine("Initial Post value: " + connection.Post);
                
                // Изменить значение Post
                connection.Post = "username=test&password=secret";
                Console.WriteLine("Updated Post value: " + connection.Post);
                
                // Очистить значение Post
                connection.Post = string.Empty;
                Console.WriteLine("Cleared Post value: " + connection.Post);
                
                // Сохраните книгу
                workbook.Save("WebQueryConnectionPostDemo.xlsx");
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


