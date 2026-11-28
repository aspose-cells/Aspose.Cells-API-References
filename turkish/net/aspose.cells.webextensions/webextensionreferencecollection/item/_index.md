---
title: "WebExtensionReferenceCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtensionReferenceCollection özelliği. Belirli bir indeksle web uzantısını alır"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensionreferencecollection/item/
---
## WebExtensionReferenceCollection indexer

Web uzantısını belirli bir dizine göre alır.

```csharp
public WebExtensionReference this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Dönüş Değeri

Web uzantısı

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionReferenceCollectionPropertyItemDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir WebExtensionReferenceCollection oluşturun
                WebExtensionReferenceCollection references = new WebExtensionReferenceCollection();
                
                // Yeni bir web uzantısı referansı ekle.
                int index = references.Add();
                
                // Belirtilen indeksdeki referansı almak için Item özelliğine (yalnızca okunur) erişin
                WebExtensionReference reference = references[index];
                
                // Alınan referans hakkında bilgi göster
                Console.WriteLine($"Retrieved web extension reference at index: {index}");
                Console.WriteLine($"Reference type: {reference.GetType().Name}");
                
                // Not: Item özelliği yalnızca okunur, bu yüzden sadece değerini almayı gösteriyoruz
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating Item property: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [WebExtensionReference](../../webextensionreference/)
* class [WebExtensionReferenceCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


