---
title: "WebExtensionProperty.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtensionProperty. Получает и задает значение пользовательского свойства"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionproperty/value/
---
## WebExtensionProperty.Value property

Получает и задает значение пользовательского свойства.

```csharp
public string Value { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // Создать экземпляр WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));

                // Установить и продемонстрировать свойство Value
                property.Value = "SampleValue123";
                Console.WriteLine($"Initial Value: {property.Value}");

                // Изменить и показать обновленное значение
                property.Value = "UpdatedValue456";
                Console.WriteLine($"Modified Value: {property.Value}");
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

* class [WebExtensionProperty](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


