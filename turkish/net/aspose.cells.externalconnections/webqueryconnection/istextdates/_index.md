---
title: "WebQueryConnection.IsTextDates"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebQueryConnection özelliği. Tarihlerin hücrelere tarih olarak değil, metin olarak aktarılıp aktarılmayacağını belirten bayrak"
type: docs
url: /tr/net/aspose.cells.externalconnections/webqueryconnection/istextdates/
---
## WebQueryConnection.IsTextDates property

Tarihlerin, çalışma sayfasındaki hücrelere tarih olarak değil metin olarak aktarılması gerektiğini gösteren işaret.

```csharp
public bool IsTextDates { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsTextDatesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // İlk çalışma sayfasına eriş
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Mevcut bir dosyadan yükleyerek bir web sorgu bağlantısı oluşturun
                // veya mevcut bir bağlantıya erişerek
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // İlk IsTextDates değerini göster
                    Console.WriteLine("Initial IsTextDates value: " + connection.IsTextDates);
                    
                    // IsTextDates'i true olarak ayarla
                    connection.IsTextDates = true;
                    Console.WriteLine("Updated IsTextDates value: " + connection.IsTextDates);
                    
                    // IsTextDates'i tekrar false olarak ayarla
                    connection.IsTextDates = false;
                    Console.WriteLine("Final IsTextDates value: " + connection.IsTextDates);
                    
                    // Web sorgu bağlantısı ile çalışma kitabını kaydedin
                    workbook.Save("WebQueryConnectionIsTextDatesDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
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


