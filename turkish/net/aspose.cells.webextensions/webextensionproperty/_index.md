---
title: "Sınıf WebExtensionProperty"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.WebExtensions.WebExtensionProperty sınıfı. Bir Office Eklentisi özel özelliğini temsil eder."
type: docs
url: /tr/net/aspose.cells.webextensions/webextensionproperty/
---
## WebExtensionProperty class

Bir Office Add-in özel özelliğinin temsilidir.

```csharp
public class WebExtensionProperty
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Name](../../aspose.cells.webextensions/webextensionproperty/name/) { get; set; } | Özel bir özellik adını alır ve ayarlar. |
| [Value](../../aspose.cells.webextensions/webextensionproperty/value/) { get; set; } | Özel bir özellik değerini alır ve ayarlar. |

### Örnekler

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
                // WebExtensionProperty'nin yeni bir örneğini oluşturun
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));
                
                // Özellik değerlerini ayarlayın
                property.Name = "SampleProperty";
                property.Value = "SampleValue";
                
                // Özellik değerlerini göster
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

### Ayrıca Bakınız

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


