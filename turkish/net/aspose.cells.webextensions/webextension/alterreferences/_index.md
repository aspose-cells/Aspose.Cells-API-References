---
title: "WebExtension.AlterReferences"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtension özelliği. Değiştirilmiş referansların bir listesini alır"
type: docs
url: /tr/net/aspose.cells.webextensions/webextension/alterreferences/
---
## WebExtension.AlterReferences property

Değiştirilen referansların bir listesini alır.

```csharp
public WebExtensionReferenceCollection AlterReferences { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyAlterReferencesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Çalışma kitabından web uzantıları koleksiyonunu al
                var webExtensions = workbook.Worksheets.WebExtensions;
                
                // Yeni bir web uzantısı ekleyin
                int index = webExtensions.Add();
                WebExtension webExtension = webExtensions[index];
                
                // AlterReferences özelliğine erişin (yalnızca okunur)
                WebExtensionReferenceCollection alterReferences = webExtension.AlterReferences;
                
                // Alter referansları hakkında bilgi göster
                Console.WriteLine($"Number of alter references: {alterReferences.Count}");
                
                // Yeni bir alter referansı ekle (koleksiyonu kullanmayı gösterir)
                int newRefIndex = alterReferences.Add();
                Console.WriteLine($"Added new alter reference at index: {newRefIndex}");
                
                // Güncellenmiş sayıyı göster
                Console.WriteLine($"Updated number of alter references: {alterReferences.Count}");
                
                // Çalışma kitabını kaydedin
                workbook.Save("WebExtensionAlterReferencesDemo.xlsx");
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

* class [WebExtensionReferenceCollection](../../webextensionreferencecollection/)
* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


