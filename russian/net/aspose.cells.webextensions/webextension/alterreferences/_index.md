---
title: "WebExtension.AlterReferences"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtension. Возвращает список альтернативных ссылок"
type: docs
url: /ru/net/aspose.cells.webextensions/webextension/alterreferences/
---
## WebExtension.AlterReferences property

Получает список альтернативных ссылок.

```csharp
public WebExtensionReferenceCollection AlterReferences { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyAlterReferencesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить коллекцию веб‑расширений из рабочей книги
                var webExtensions = workbook.Worksheets.WebExtensions;
                
                // Добавить новое веб-расширение
                int index = webExtensions.Add();
                WebExtension webExtension = webExtensions[index];
                
                // Доступ к свойству AlterReferences (только для чтения)
                WebExtensionReferenceCollection alterReferences = webExtension.AlterReferences;
                
                // Отобразить информацию об alter references
                Console.WriteLine($"Number of alter references: {alterReferences.Count}");
                
                // Добавить новый alter reference (демонстрирует использование коллекции)
                int newRefIndex = alterReferences.Add();
                Console.WriteLine($"Added new alter reference at index: {newRefIndex}");
                
                // Отобразить обновленное количество
                Console.WriteLine($"Updated number of alter references: {alterReferences.Count}");
                
                // Сохраните книгу
                workbook.Save("WebExtensionAlterReferencesDemo.xlsx");
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

* class [WebExtensionReferenceCollection](../../webextensionreferencecollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


