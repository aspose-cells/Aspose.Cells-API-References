---
title: "WebQueryConnection.IsXml"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebQueryConnection. true, если источник веб‑запроса — XML, а не HTML, иначе false"
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/isxml/
---
## WebQueryConnection.IsXml property

true, если источник веб‑запроса — XML (в отличие от HTML), иначе false.

```csharp
public bool IsXml { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXmlDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить доступ к первому соединению данных (предполагая, что это WebQueryConnection)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Отобразить начальное значение IsXml
                    Console.WriteLine("Initial IsXml value: " + connection.IsXml);
                    
                    // Установить IsXml в true (поскольку оно поддерживает чтение‑запись)
                    connection.IsXml = true;
                    Console.WriteLine("Updated IsXml value: " + connection.IsXml);
                    
                    // Установить IsXml обратно в false
                    connection.IsXml = false;
                    Console.WriteLine("Final IsXml value: " + connection.IsXml);
                    
                    // Сохраните книгу
                    workbook.Save("WebQueryConnectionIsXmlDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
                }
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


