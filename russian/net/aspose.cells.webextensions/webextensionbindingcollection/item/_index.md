---
title: "WebExtensionBindingCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtensionBindingCollection. Получает связь привязки веб‑расширения по указанному индексу"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionbindingcollection/item/
---
## WebExtensionBindingCollection indexer

Получает связь привязки веб-расширения по указанному индексу.

```csharp
public WebExtensionBinding this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Возвращаемое значение

Связь привязки веб‑расширения

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать коллекцию привязок веб‑расширения
            WebExtensionBindingCollection bindingCollection = new WebExtensionBindingCollection();

            // Добавить новую привязку в коллекцию
            int index = bindingCollection.Add();

            // Получить доступ к привязке с помощью свойства Item (только для чтения)
            WebExtensionBinding binding = bindingCollection[index];

            // Установить свойства привязки
            binding.Id = "binding1";
            binding.Type = "Text";
            binding.Appref = "Sheet1!A1";

            // Отобразить детали привязки
            Console.WriteLine("Binding ID: " + binding.Id);
            Console.WriteLine("Binding Type: " + binding.Type);
            Console.WriteLine("Binding AppRef: " + binding.Appref);

            // Изменить привязку через коллекцию
            bindingCollection[index].Id = "modifiedBinding";
            Console.WriteLine("Modified Binding ID: " + bindingCollection[index].Id);

            // Сохраните книгу
            workbook.Save("WebExtensionBindingDemo.xlsx");
        }
    }
}
```

### См. также

* class [WebExtensionBinding](../../webextensionbinding/)
* class [WebExtensionBindingCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


