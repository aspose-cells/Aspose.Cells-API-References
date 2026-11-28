---
title: "WebQueryConnection.Url"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebQueryConnection özelliği. Harici verileri yenilemek için kullanılacak URL"
type: docs
url: /tr/net/aspose.cells.externalconnections/webqueryconnection/url/
---
## WebQueryConnection.Url property

Harici verileri yenilemek için kullanılacak URL.

```csharp
public string Url { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyUrlDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Web sorgu bağlantısını koleksiyona ekleyerek oluşturun
            // Koleksiyon muhtemelen bağlantı nesnesini oluşturacak ve döndürecek
            WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];

            // Web sorgusu için başlangıç URL'sini ayarlayın
            connection.Url = "https://example.com/data.html";
            Console.WriteLine("Initial URL: " + connection.Url);

            // URL'yi farklı bir kaynağa değiştirin
            connection.Url = "https://example.com/updated-data.xml";
            Console.WriteLine("Updated URL: " + connection.Url);

            // Bağlantıyı XML verisini ayrıştıracak şekilde yapılandırın
            connection.IsXml = true;

            // Veri bağlantısını yenileyin (normalde URL'den veri alır)
            // Not: Gerçek web erişimi ağ bağlantısı gerektirir
            // workbook.RefreshAllConnections();

            // Web sorgu bağlantısı ile çalışma kitabını kaydedin
            workbook.Save("WebQueryConnectionUrlDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


