---
title: "WebExtensionProperty.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtensionProperty özelliği. Özel bir özellik adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensionproperty/name/
---
## WebExtensionProperty.Name property

Özel bir özellik adını alır ve ayarlar.

```csharp
public string Name { get; set; }
```

### Örnekler

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
                // Bir WebExtensionProperty örneği oluştur
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));

                // Name özelliğini ayarla ve göster
                property.Name = "SampleName";
                Console.WriteLine($"Initial Name: {property.Name}");

                // Güncellenmiş adı değiştir ve görüntüle
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

### Ayrıca Bakınız

* class [WebExtensionProperty](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


