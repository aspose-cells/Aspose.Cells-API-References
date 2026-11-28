---
title: "Sınıf WebExtensionBinding"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.WebExtensions.WebExtensionBinding sınıfı. Bir Office Eklentisi ile belgedeki veri arasındaki bağlama ilişkisini temsil eder"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensionbinding/
---
## WebExtensionBinding class

Bir Office Add-in ile belgedeki veri arasındaki bağlama ilişkisinin temsilidir.

```csharp
public class WebExtensionBinding
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [WebExtensionBinding](webextensionbinding/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Appref](../../aspose.cells.webextensions/webextensionbinding/appref/) { get; set; } | Bu listedeki bağlama girişini belgede bağlanan veriyle eşleştirmek için kullanılan bağlama anahtarını alır ve ayarlar. |
| [Id](../../aspose.cells.webextensions/webextensionbinding/id/) { get; set; } | Bağlama tanımlayıcısını alır ve ayarlar. |
| [Type](../../aspose.cells.webextensions/webextensionbinding/type/) { get; set; } | Bağlama türünü alır ve ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionBindingDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir WebExtensionBinding örneği oluşturun
                WebExtensionBinding binding = new WebExtensionBinding();

                // Özellikleri ayarla
                binding.Id = "DemoBinding";
                binding.Type = "range";
                binding.Appref = "Sheet1!A1";

                // Özellik değerlerini göster
                Console.WriteLine($"Binding created - ID: {binding.Id}, Type: {binding.Type}, Appref: {binding.Appref}");

                // Özellikleri değiştir.
                binding.Appref = "Sheet1!B2";
                Console.WriteLine($"Updated Appref: {binding.Appref}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebExtensionBinding: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


