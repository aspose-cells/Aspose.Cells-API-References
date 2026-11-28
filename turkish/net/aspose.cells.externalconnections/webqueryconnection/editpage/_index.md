---
title: "WebQueryConnection.EditPage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebQueryConnection özelliği. Web sorgu verilerini gösteren kullanıcıya yönelik web sayfasının URL'si. Bu URL, sourceDatatrue ve url'nin bir XML dosyasına yönlendirilmesi durumunda saklanır. Böylece kullanıcı sayfası UI'da gösterilebilir ve XML verileri arka planda alınabilir."
type: docs
url: /tr/net/aspose.cells.externalconnections/webqueryconnection/editpage/
---
## WebQueryConnection.EditPage property

Web sorgu verilerini gösteren kullanıcıya yönelik web sayfasının URL'si. sourceData="true" olduğu ve url'nin bir XML dosyasına yönlendirildiği durumda bu URL korunur. Böylece kullanıcıya yönelik sayfa UI'da gösterilebilir ve XML verisi arka planda alınabilir.

```csharp
[Obsolete("Use WebQueryConnection.EditWebPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EditPage { get; set; }
```

### Açıklamalar

NOTE: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen WebQueryConnection.EditWebPage özelliğini kullanın. Bu özellik Ekim 2017'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyEditPageDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Mevcutsa ilk mevcut web sorgu bağlantısına erişin
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // İlk EditPage değerini görüntüle
                    Console.WriteLine("Initial EditPage value: " + connection.EditPage);
                    
                    // EditPage'i yeni bir URL'ye ayarla (okuma-yazma olduğu için)
                    connection.EditPage = "https://example.com/editpage";
                    Console.WriteLine("Updated EditPage value: " + connection.EditPage);
                    
                    // Çalışma kitabını kaydedin
                    workbook.Save("WebQueryConnectionEditPageDemo.xlsx");
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


