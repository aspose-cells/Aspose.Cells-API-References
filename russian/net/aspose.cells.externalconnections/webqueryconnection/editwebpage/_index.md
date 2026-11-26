---
title: "WebQueryConnection.EditWebPage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WebQueryConnection property. URL веб‑страницы, отображающей данные веб‑запроса для пользователя. Этот URL сохраняется в случае, когда sourceDatatrue и url были перенаправлены на ссылку на XML‑файл. Затем пользовательская страница может быть показана в UI, а XML‑данные могут быть получены в фоновом режиме."
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/editwebpage/
---
## WebQueryConnection.EditWebPage property

URL пользовательской веб‑страницы, отображающей данные веб‑запроса. Этот URL сохраняется в случае, когда sourceData="true" и url был перенаправлен к XML‑файлу. Затем пользовательская страница может быть показана в интерфейсе, а XML‑данные могут быть получены в фоновом режиме.

```csharp
public string EditWebPage { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditWebPageDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получите первое существующее подключение веб‑запроса (если есть)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Установить начальное значение EditWebPage
                    connection.EditWebPage = "https://example.com/user-facing-page.html";
                    Console.WriteLine("Initial EditWebPage value: " + connection.EditWebPage);
                    
                    // Обновить значение EditWebPage
                    connection.EditWebPage = "https://example.com/updated-user-page.html";
                    Console.WriteLine("Updated EditWebPage value: " + connection.EditWebPage);
                    
                    // Сохраните книгу с подключением веб‑запроса
                    workbook.Save("WebQueryConnectionEditWebPageDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
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


