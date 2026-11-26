---
title: "WebExtensionBinding.Appref"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtensionBinding. Получает и задает ключ привязки, используемый для сопоставления записи привязки в этом списке с привязанными данными в документе"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionbinding/appref/
---
## WebExtensionBinding.Appref property

Получает и задает ключ привязки, используемый для сопоставления записи привязки в этом списке с привязанными данными в документе.

```csharp
public string Appref { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingPropertyApprefDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новый экземпляр WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Установите свойства, включая Appref
                binding.Id = "Binding1";
                binding.Type = "text";
                binding.Appref = "Sheet1!A1:B2";
                
                // Отобразить текущее значение Appref
                Console.WriteLine("Appref value: " + binding.Appref);
                
                // Изменить значение Appref, чтобы продемонстрировать его чтение/запись
                binding.Appref = "Sheet1!C3:D4";
                Console.WriteLine("Updated Appref value: " + binding.Appref);
                
                Console.WriteLine("Appref property has been successfully demonstrated");
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


