---
title: "WebQueryConnection.ConnectionFile"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebQueryConnection özelliği. Bağlantı dosyasını alır"
type: docs
url: /tr/net/aspose.cells.externalconnections/webqueryconnection/connectionfile/
---
## WebQueryConnection.ConnectionFile property

Bağlantı dosyasını alır.

```csharp
public override string ConnectionFile { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyConnectionFileDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Web sorgu verileriyle örnek bir çalışma sayfası oluştur
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Sample Web Query Data";
                
                // İlk mevcut web sorgu bağlantısını al (varsa)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // ConnectionFile değerini göster (yalnızca okunabilir özellik)
                    Console.WriteLine("ConnectionFile value: " + connection.ConnectionFile);
                    
                    // Çalışma kitabını kaydedin
                    workbook.Save("WebQueryConnectionFileDemo.xlsx");
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


