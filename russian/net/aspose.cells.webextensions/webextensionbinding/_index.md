---
title: "Класс WebExtensionBinding"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.WebExtensions.WebExtensionBinding class. Представляет связь привязки между надстройкой Office и данными в документе"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionbinding/
---
## WebExtensionBinding class

Представляет связь привязки между надстройкой Office и данными в документе.

```csharp
public class WebExtensionBinding
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WebExtensionBinding](webextensionbinding/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Appref](../../aspose.cells.webextensions/webextensionbinding/appref/) { get; set; } | Получает и задает ключ привязки, используемый для сопоставления записи привязки в этом списке с привязанными данными в документе. |
| [Id](../../aspose.cells.webextensions/webextensionbinding/id/) { get; set; } | Получает и задает идентификатор привязки. |
| [Type](../../aspose.cells.webextensions/webextensionbinding/type/) { get; set; } | Получает и задает тип привязки. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionBindingDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новый экземпляр WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();

                // Установить свойства
                binding.Id = "DemoBinding";
                binding.Type = "range";
                binding.Appref = "Sheet1!A1";

                // Отобразить значения свойств
                Console.WriteLine($"Binding created - ID: {binding.Id}, Type: {binding.Type}, Appref: {binding.Appref}");

                // Изменить свойства
                binding.Appref = "Sheet1!B2";
                Console.WriteLine($"Updated Appref: {binding.Appref}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionBinding: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


