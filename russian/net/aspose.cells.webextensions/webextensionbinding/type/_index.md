---
title: "WebExtensionBinding.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtensionBinding. Получает и задает тип привязки"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionbinding/type/
---
## WebExtensionBinding.Type property

Получает и задает тип привязки.

```csharp
public string Type { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingPropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новый экземпляр WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Установить свойство Type
                binding.Type = "text";
                
                // Отобразить текущее значение Type
                Console.WriteLine("Initial Type value: " + binding.Type);
                
                // Изменить значение Type, чтобы продемонстрировать его чтение/запись
                binding.Type = "range";
                Console.WriteLine("Updated Type value: " + binding.Type);
                
                Console.WriteLine("Type property has been successfully demonstrated");
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


