---
title: "WebExtension.Id"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtension özelliği. Geçerli belgede Office Eklentisi örneğini benzersiz şekilde tanımlayan değeri alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.webextensions/webextension/id/
---
## WebExtension.Id property

Geçerli belgede Office Eklentisi örneğini benzersiz şekilde tanımlayan değeri alır ve ayarlar.

```csharp
public string Id { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Çalışma kitabından web uzantıları koleksiyonunu al
                var webExtensions = workbook.Worksheets.WebExtensions;
                
                // Yeni bir web uzantısı ekle (gerekli parametrelerle oluşturulacaktır)
                int index = webExtensions.Add();
                WebExtension webExtension = webExtensions[index];
                
                // Id özelliğini ayarla (çünkü okuma-yazma özelliğine sahiptir)
                webExtension.Id = "SampleAddin123";
                
                // Id özelliğinin mevcut değerini göster
                Console.WriteLine($"WebExtension Id: {webExtension.Id}");
                
                // Id özelliğini değiştirerek yazılabilir olduğunu göster
                webExtension.Id = "UpdatedAddin456";
                Console.WriteLine($"Updated WebExtension Id: {webExtension.Id}");
                
                // Çalışma kitabını kaydedin
                workbook.Save("WebExtensionIdDemo.xlsx");
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

* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


