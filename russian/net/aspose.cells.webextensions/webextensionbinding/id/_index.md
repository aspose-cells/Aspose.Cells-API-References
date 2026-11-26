---
title: "WebExtensionBinding.Id"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtensionBinding. Получает и задает идентификатор привязки"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionbinding/id/
---
## WebExtensionBinding.Id property

Получает и задает идентификатор привязки.

```csharp
public string Id { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingPropertyIdDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новый экземпляр WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Установить свойство Id
                binding.Id = "SampleBindingId";
                
                // Отобразить текущее значение Id
                Console.WriteLine("Initial Id value: " + binding.Id);
                
                // Изменить значение Id, чтобы продемонстрировать его чтение/запись
                binding.Id = "UpdatedBindingId";
                Console.WriteLine("Updated Id value: " + binding.Id);
                
                Console.WriteLine("Id property has been successfully demonstrated");
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

* class [WebExtensionBinding](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


