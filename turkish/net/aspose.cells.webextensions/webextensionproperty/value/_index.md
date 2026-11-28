---
title: "WebExtensionProperty.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtensionProperty özelliği. Özel bir özellik değerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensionproperty/value/
---
## WebExtensionProperty.Value property

Özel bir özellik değerini alır ve ayarlar.

```csharp
public string Value { get; set; }
```

### Örnekler

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
                // Bir WebExtensionProperty örneği oluştur
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));

                // Value özelliğini ayarla ve göster
                property.Value = "SampleValue123";
                Console.WriteLine($"Initial Value: {property.Value}");

                // Güncellenmiş değeri değiştir ve göster
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

### Ayrıca Bakınız

* class [WebExtensionProperty](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


