---
title: "WebExtension.Id"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtension. Получает и задает уникальный идентификатор экземпляра надстройки Office в текущем документе"
type: docs
url: /ru/net/aspose.cells.webextensions/webextension/id/
---
## WebExtension.Id property

Получает и задает уникальный идентификатор экземпляра Office Add-in в текущем документе.

```csharp
public string Id { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить коллекцию веб‑расширений из рабочей книги
                var webExtensions = workbook.Worksheets.WebExtensions;
                
                // Добавить новое веб‑расширение (это создаст его с необходимыми параметрами)
                int index = webExtensions.Add();
                WebExtension webExtension = webExtensions[index];
                
                // Установить свойство Id (поскольку оно доступно для чтения и записи)
                webExtension.Id = "SampleAddin123";
                
                // Отобразить текущее значение свойства Id
                Console.WriteLine($"WebExtension Id: {webExtension.Id}");
                
                // Изменить свойство Id, чтобы продемонстрировать возможность записи
                webExtension.Id = "UpdatedAddin456";
                Console.WriteLine($"Updated WebExtension Id: {webExtension.Id}");
                
                // Сохраните книгу
                workbook.Save("WebExtensionIdDemo.xlsx");
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

* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


