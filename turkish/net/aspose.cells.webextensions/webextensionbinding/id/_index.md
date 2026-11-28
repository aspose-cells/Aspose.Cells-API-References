---
title: "WebExtensionBinding.Id"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtensionBinding özelliği. Bağlama tanımlayıcısını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensionbinding/id/
---
## WebExtensionBinding.Id property

Bağlama tanımlayıcısını alır ve ayarlar.

```csharp
public string Id { get; set; }
```

### Örnekler

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
                // Yeni bir WebExtensionBinding örneği oluşturun
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Id özelliğini ayarla
                binding.Id = "SampleBindingId";
                
                // Id'nin mevcut değerini göster
                Console.WriteLine("Initial Id value: " + binding.Id);
                
                // Id değerini değiştirerek okuma/yazma olduğunu göster
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

### Ayrıca Bakınız

* class [WebExtensionBinding](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


