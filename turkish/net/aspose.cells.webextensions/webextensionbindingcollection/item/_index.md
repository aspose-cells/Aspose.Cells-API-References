---
title: "WebExtensionBindingCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtensionBindingCollection özelliği. Belirli indeks ile web uzantısı bağlama ilişkisini alır"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensionbindingcollection/item/
---
## WebExtensionBindingCollection indexer

Belirli bir indeks ile web uzantısı bağlama ilişkisini alır.

```csharp
public WebExtensionBinding this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Dönüş Değeri

Web uzantısı bağlama ilişkisi

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir web uzantısı bağlama koleksiyonu oluştur
            WebExtensionBindingCollection bindingCollection = new WebExtensionBindingCollection();

            // Koleksiyona yeni bir bağlama ekle
            int index = bindingCollection.Add();

            // Item özelliğini (yalnızca okuma) kullanarak bağlamaya eriş
            WebExtensionBinding binding = bindingCollection[index];

            // Bağlama üzerinde özellikleri ayarla
            binding.Id = "binding1";
            binding.Type = "Text";
            binding.Appref = "Sheet1!A1";

            // Bağlama ayrıntılarını göster
            Console.WriteLine("Binding ID: " + binding.Id);
            Console.WriteLine("Binding Type: " + binding.Type);
            Console.WriteLine("Binding AppRef: " + binding.Appref);

            // Koleksiyon aracılığıyla bağlamayı değiştir
            bindingCollection[index].Id = "modifiedBinding";
            Console.WriteLine("Modified Binding ID: " + bindingCollection[index].Id);

            // Çalışma kitabını kaydedin
            workbook.Save("WebExtensionBindingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WebExtensionBinding](../../webextensionbinding/)
* class [WebExtensionBindingCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


