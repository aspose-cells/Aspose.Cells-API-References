---
title: "WebQueryConnection.IsParsePre"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebQueryConnection özelliği. Web sayfasındaki HTML PRE etiketleri içinde bulunan verilerin, sayfayı bir sorgu tablosuna içe aktardığınızda sütunlara ayrılıp ayrılmayacağını gösteren bayrak"
type: docs
url: /tr/net/aspose.cells.externalconnections/webqueryconnection/isparsepre/
---
## WebQueryConnection.IsParsePre property

Web sayfasındaki HTML PRE etiketleri içinde bulunan verilerin, sayfa bir sorgu tablosuna içe aktarıldığında sütunlara ayrılıp ayrılmayacağını gösteren işaret.

```csharp
public bool IsParsePre { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsParsePreDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Çalışma kitabındaki mevcut bağlantıyı kullanarak yeni bir web sorgu bağlantısı oluştur
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
                
                // İlk IsParsePre değerini göster (varsayılan)
                Console.WriteLine("Initial IsParsePre value: " + connection.IsParsePre);
                
                // IsParsePre'i true olarak ayarla
                connection.IsParsePre = true;
                Console.WriteLine("Updated IsParsePre value: " + connection.IsParsePre);
                
                // IsParsePre'yi false olarak geri ayarla
                connection.IsParsePre = false;
                Console.WriteLine("Final IsParsePre value: " + connection.IsParsePre);
                
                // Çalışma kitabını kaydedin
                workbook.Save("WebQueryConnectionIsParsePreDemo.xlsx");
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


