---
title: "WebExtensionReferenceCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtensionReferenceCollection. Получает веб‑расширение по конкретному индексу"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionreferencecollection/item/
---
## WebExtensionReferenceCollection indexer

Получает веб‑расширение по конкретному индексу.

```csharp
public WebExtensionReference this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Возвращаемое значение

Веб‑расширение

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionReferenceCollectionPropertyItemDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте новую WebExtensionReferenceCollection
                WebExtensionReferenceCollection references = new WebExtensionReferenceCollection();
                
                // Добавьте новую ссылку на веб‑расширение
                int index = references.Add();
                
                // Получите свойство Item (только для чтения), чтобы получить ссылку по указанному индексу
                WebExtensionReference reference = references[index];
                
                // Отобразите информацию о полученной ссылке
                Console.WriteLine($"Retrieved web extension reference at index: {index}");
                Console.WriteLine($"Reference type: {reference.GetType().Name}");
                
                // Примечание: свойство Item только для чтения, поэтому мы только демонстрируем получение его значения
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating Item property: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtensionReferenceCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


