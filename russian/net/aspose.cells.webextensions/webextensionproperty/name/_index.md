---
title: "WebExtensionProperty.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebExtensionProperty. Получает и задает имя пользовательского свойства"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionproperty/name/
---
## WebExtensionProperty.Name property

Получает и задает имя пользовательского свойства.

```csharp
public string Name { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyPropertyNameDemo
    {
        public static void Run()
        {
            try
            {
                // Создать экземпляр WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));

                // Установить и продемонстрировать свойство Name
                property.Name = "SampleName";
                Console.WriteLine($"Initial Name: {property.Name}");

                // Изменить и отобразить обновленное имя
                property.Name = "UpdatedName";
                Console.WriteLine($"Modified Name: {property.Name}");
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


