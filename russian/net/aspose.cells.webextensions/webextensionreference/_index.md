---
title: "Класс WebExtensionReference"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.WebExtensions.WebExtensionReference. Представляет идентификацию местоположения поставщика и версии расширения"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionreference/
---
## WebExtensionReference class

Представляет идентификацию местоположения поставщика и версии расширения.

```csharp
public class WebExtensionReference
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Id](../../aspose.cells.webextensions/webextensionreference/id/) { get; set; } | Получает и задает идентификатор, связанный с Office Add-in в провайдере каталога. Идентификатор ДОЛЖЕН быть уникальным в пределах провайдера каталога. |
| [StoreName](../../aspose.cells.webextensions/webextensionreference/storename/) { get; set; } | Получает и задает экземпляр маркетплейса, где хранится Office Add-in. |
| [StoreType](../../aspose.cells.webextensions/webextensionreference/storetype/) { get; set; } | Получает и задает тип маркетплейса, который определяет атрибут хранилища. |
| [Version](../../aspose.cells.webextensions/webextensionreference/version/) { get; set; } | Получает и задает версию. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionReferenceDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Сначала создайте WebExtension
                WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
                int extensionIndex = webExtensions.Add();
                WebExtension webExt = webExtensions[extensionIndex];

                // Получите WebExtensionReference из WebExtension
                WebExtensionReference webExtensionRef = webExt.Reference;

                // Установите свойства WebExtensionReference
                webExtensionRef.Id = "my-addin-123";
                webExtensionRef.Version = "1.0.0";
                webExtensionRef.StoreName = "MyAddinStore";
                webExtensionRef.StoreType = WebExtensionStoreType.OMEX;

                // Отобразите свойства ссылки
                Console.WriteLine($"WebExtension Reference created:");
                Console.WriteLine($"ID: {webExtensionRef.Id}");
                Console.WriteLine($"Version: {webExtensionRef.Version}");
                Console.WriteLine($"Store Name: {webExtensionRef.StoreName}");
                Console.WriteLine($"Store Type: {webExtensionRef.StoreType}");

                // Сохраните книгу
                workbook.Save("WebExtensionReferenceDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with WebExtension reference.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionReference: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


