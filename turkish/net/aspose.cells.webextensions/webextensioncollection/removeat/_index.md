---
title: "WebExtensionCollection.RemoveAt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebExtensionCollection yöntemi. Web uzantısını indeksle kaldırır"
type: docs
url: /tr/net/aspose.cells.webextensions/webextensioncollection/removeat/
---
## WebExtensionCollection.RemoveAt method

Web uzantısını indeksle kaldır.

```csharp
public void RemoveAt(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | İndeks. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Web uzantıları koleksiyonu oluştur
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;

            // Koleksiyona bazı web uzantıları ekleyin
            int index1 = webExtensions.Add();
            int index2 = webExtensions.Add();
            int index3 = webExtensions.Add();

            Console.WriteLine($"WebExtensions count before RemoveAt: {webExtensions.Count}");

            try
            {
                // Int32 parametresiyle RemoveAt metodunu çağırın
                webExtensions.RemoveAt(index2);
                
                Console.WriteLine("Method executed successfully with parameter (Int32)");
                Console.WriteLine($"WebExtensions count after RemoveAt: {webExtensions.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("WebExtensionCollectionMethodRemoveAtDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


