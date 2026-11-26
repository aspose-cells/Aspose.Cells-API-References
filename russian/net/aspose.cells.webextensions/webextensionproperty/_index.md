---
title: "Класс WebExtensionProperty"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.WebExtensions.WebExtensionProperty. Представляет пользовательское свойство Office Addin"
type: docs
url: /ru/net/aspose.cells.webextensions/webextensionproperty/
---
## WebExtensionProperty class

Представляет пользовательское свойство надстройки Office.

```csharp
public class WebExtensionProperty
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Name](../../aspose.cells.webextensions/webextensionproperty/name/) { get; set; } | Получает и задает имя пользовательского свойства. |
| [Value](../../aspose.cells.webextensions/webextensionproperty/value/) { get; set; } | Получает и задает значение пользовательского свойства. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionPropertyDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте новый экземпляр WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));
                
                // Установите значения свойств
                property.Name = "SampleProperty";
                property.Value = "SampleValue";
                
                // Отобразите значения свойств
                Console.WriteLine($"Property Name: {property.Name}");
                Console.WriteLine($"Property Value: {property.Value}");
                
                Console.WriteLine("WebExtensionProperty demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in WebExtensionProperty demo: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


