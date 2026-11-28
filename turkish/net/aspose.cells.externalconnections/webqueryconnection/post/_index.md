---
title: "WebQueryConnection.Post"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebQueryConnection özelliği. Web sorgusundan veri döndürmek için bir web sunucusuna veri gönderirken kullanılan post yöntemiyle ilgili dizeyi döndürür veya ayarlar"
type: docs
url: /tr/net/aspose.cells.externalconnections/webqueryconnection/post/
---
## WebQueryConnection.Post property

Bir web sorgusundan veri döndürmek için verileri bir web sunucusuna gönderirken kullanılan post yöntemiyle kullanılan dizeyi alır veya ayarlar.

```csharp
public string Post { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyPostDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Mevcut bir bağlantıya erişerek veya uygun başlatma ile oluşturarak bir web sorgu bağlantısı oluşturun
                // WebQueryConnection'ı doğrudan örnekleyemediğimiz için, mevcutsa ilk bağlantıyı kullanacağız
                WebQueryConnection connection = null;
                
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection webQueryConn)
                {
                    connection = webQueryConn;
                }
                else
                {
                    // Bağlantı yoksa, bir taklit bağlantı ile gösterim yapacağız
                    Console.WriteLine("No existing web query connection found - demonstrating with property access only");
                    return;
                }
                
                // İlk Post değerini ayarla
                connection.Post = "param1=value1&param2=value2";
                Console.WriteLine("Initial Post value: " + connection.Post);
                
                // Post değerini değiştir
                connection.Post = "username=test&password=secret";
                Console.WriteLine("Updated Post value: " + connection.Post);
                
                // Post değerini temizle
                connection.Post = string.Empty;
                Console.WriteLine("Cleared Post value: " + connection.Post);
                
                // Çalışma kitabını kaydedin
                workbook.Save("WebQueryConnectionPostDemo.xlsx");
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


