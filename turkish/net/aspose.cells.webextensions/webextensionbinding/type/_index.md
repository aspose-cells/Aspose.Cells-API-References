---
title: "WebExtensionBinding.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtensionBinding özelliği. Bağlama türünü alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensionbinding/type/
---
## WebExtensionBinding.Type property

Bağlama türünü alır ve ayarlar.

```csharp
public string Type { get; set; }
```

### Örnekler

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
                // Yeni bir WebExtensionBinding örneği oluşturun
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Type özelliğini ayarla
                binding.Type = "text";
                
                // Type'ın mevcut değerini göster
                Console.WriteLine("Initial Type value: " + binding.Type);
                
                // Type değerini değiştirerek okuma/yazma olduğunu göster
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

### Ayrıca Bakınız

* class [WebExtensionBinding](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


