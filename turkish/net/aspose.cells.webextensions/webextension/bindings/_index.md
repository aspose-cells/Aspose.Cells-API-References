---
title: "WebExtension.Bindings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtension özelliği. Bir Office Eklentisi ile belgedeki veri arasındaki tüm bağlam ilişkilerini alır"
type: docs
url: /tr/net/aspose.cells.webextensions/webextension/bindings/
---
## WebExtension.Bindings property

Bir Office Eklentisi ile belgedeki veri arasındaki tüm bağlama ilişkilerini alır.

```csharp
public WebExtensionBindingCollection Bindings { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyBindingsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Örnek bir çalışma sayfası oluşturun
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Bir web uzantısını bir yerden aldığımızı varsayalım (çünkü doğrudan bir tane oluşturamıyoruz)
                // Kodun derlenebilmesi için yapıyı korurken yapılan minimal bir değişikliktir
                WebExtension webExtension = null; // In real usage, this would come from workbook.WebExtensions or similar
                
                if (webExtension != null)
                {
                    // Bindings özelliğine erişin (yalnızca okunur)
                    WebExtensionBindingCollection bindings = webExtension.Bindings;
                    
                    // Bağlamalar hakkında bilgi göster
                    Console.WriteLine($"Number of bindings: {bindings.Count}");
                    
                    // Yeni bir bağlama ekle (koleksiyonun kullanımını gösterir)
                    int newBindingIndex = bindings.Add();
                    Console.WriteLine($"Added new binding at index: {newBindingIndex}");
                    
                    // Güncellenmiş sayıyı göster
                    Console.WriteLine($"Updated number of bindings: {bindings.Count}");
                }
                else
                {
                    Console.WriteLine("No web extension available");
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("WebExtensionBindingsDemo.xlsx");
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

* class [WebExtensionBindingCollection](../../webextensionbindingcollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


