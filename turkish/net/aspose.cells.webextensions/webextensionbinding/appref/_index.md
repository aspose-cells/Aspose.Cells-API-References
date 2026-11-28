---
title: "WebExtensionBinding.Appref"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtensionBinding özelliği. Bu listedeki bağlama girişini belgede bağlanan veriyle eşleştirmek için kullanılan bağlama anahtarını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensionbinding/appref/
---
## WebExtensionBinding.Appref property

Bu listedeki bağlama girişini belgede bağlanan veriyle eşleştirmek için kullanılan bağlama anahtarını alır ve ayarlar.

```csharp
public string Appref { get; set; }
```

### Örnekler

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
                // Yeni bir WebExtensionBinding örneği oluşturun
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Appref dahil olmak üzere özellikleri ayarlayın
                binding.Id = "Binding1";
                binding.Type = "text";
                binding.Appref = "Sheet1!A1:B2";
                
                // Appref'in mevcut değerini göster
                Console.WriteLine("Appref value: " + binding.Appref);
                
                // Appref değerini değiştirerek okuma/yazma olduğunu göster
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

### Ayrıca Bakınız

* class [WebExtensionBinding](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


