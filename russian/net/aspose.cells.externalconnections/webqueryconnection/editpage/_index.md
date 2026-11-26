---
title: "WebQueryConnection.EditPage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "WebQueryConnection property. URL веб‑страницы, отображающей данные веб‑запроса для пользователя. Этот URL сохраняется в случае, когда sourceDatatrue и url были перенаправлены на ссылку на XML‑файл. Затем пользовательская страница может быть показана в UI, а XML‑данные могут быть получены в фоновом режиме."
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/editpage/
---
## WebQueryConnection.EditPage property

URL пользовательской веб‑страницы, отображающей данные веб‑запроса. Этот URL сохраняется в случае, когда sourceData="true" и url был перенаправлен к XML‑файлу. Затем пользовательская страница может быть показана в интерфейсе, а XML‑данные могут быть получены в фоновом режиме.

```csharp
[Obsolete("Use WebQueryConnection.EditWebPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EditPage { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство WebQueryConnection.EditWebPage. Это свойство будет удалено через 12 месяцев, начиная с октября 2017 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditPageDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить первое существующее соединение веб‑запроса, если оно доступно
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Отобразить начальное значение EditPage
                    Console.WriteLine("Initial EditPage value: " + connection.EditPage);
                    
                    // Установить EditPage в новый URL (поскольку оно поддерживает чтение‑запись)
                    connection.EditPage = "https://example.com/editpage";
                    Console.WriteLine("Updated EditPage value: " + connection.EditPage);
                    
                    // Сохраните книгу
                    workbook.Save("WebQueryConnectionEditPageDemo.xlsx");
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


