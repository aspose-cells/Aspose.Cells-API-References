---
title: "WebQueryConnection.IsParsePre"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WebQueryConnection property. Флаг, указывающий, следует ли парсить данные, содержащиеся внутри тегов HTML PRE на веб‑странице, в столбцы при импорте страницы в таблицу запросов"
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/isparsepre/
---
## WebQueryConnection.IsParsePre property

Флаг, указывающий, разбираются ли данные, содержащиеся внутри тегов HTML PRE на веб‑странице, в столбцы при импорте страницы в таблицу запросов.

```csharp
public bool IsParsePre { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsParsePreDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Создать новое соединение веб‑запроса, используя существующее соединение из рабочей книги
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
                
                // Отобразить начальное значение IsParsePre (по умолчанию)
                Console.WriteLine("Initial IsParsePre value: " + connection.IsParsePre);
                
                // Установить IsParsePre в true
                connection.IsParsePre = true;
                Console.WriteLine("Updated IsParsePre value: " + connection.IsParsePre);
                
                // Установить IsParsePre обратно в false
                connection.IsParsePre = false;
                Console.WriteLine("Final IsParsePre value: " + connection.IsParsePre);
                
                // Сохраните книгу
                workbook.Save("WebQueryConnectionIsParsePreDemo.xlsx");
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


