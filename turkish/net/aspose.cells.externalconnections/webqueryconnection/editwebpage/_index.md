---
title: "WebQueryConnection.EditWebPage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebQueryConnection özelliği. Web sorgu verilerini gösteren kullanıcıya yönelik web sayfasının URL'si. Bu URL, sourceDatatrue ve url'nin bir XML dosyasına yönlendirilmesi durumunda saklanır. Böylece kullanıcı sayfası UI'da gösterilebilir ve XML verileri arka planda alınabilir."
type: docs
url: /tr/net/aspose.cells.externalconnections/webqueryconnection/editwebpage/
---
## WebQueryConnection.EditWebPage property

Web sorgu verilerini gösteren kullanıcıya yönelik web sayfasının URL'si. sourceData="true" olduğu ve url'nin bir XML dosyasına yönlendirildiği durumda bu URL korunur. Böylece kullanıcıya yönelik sayfa UI'da gösterilebilir ve XML verisi arka planda alınabilir.

```csharp
public string EditWebPage { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditWebPageDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Mevcut ilk web sorgu bağlantısına erişin (varsa)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // İlk EditWebPage değerini ayarla
                    connection.EditWebPage = "https://example.com/user-facing-page.html";
                    Console.WriteLine("Initial EditWebPage value: " + connection.EditWebPage);
                    
                    // EditWebPage değerini güncelle
                    connection.EditWebPage = "https://example.com/updated-user-page.html";
                    Console.WriteLine("Updated EditWebPage value: " + connection.EditWebPage);
                    
                    // Web sorgu bağlantısı ile çalışma kitabını kaydedin
                    workbook.Save("WebQueryConnectionEditWebPageDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
                }
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

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


