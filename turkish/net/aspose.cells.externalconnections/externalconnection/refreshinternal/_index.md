---
title: "ExternalConnection.RefreshInternal"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. Bağlantının otomatik yenilenmeleri arasındaki dakika sayısını belirtir"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/refreshinternal/
---
## ExternalConnection.RefreshInternal property

Bağlantının otomatik yenilemeleri arasındaki dakika sayısını belirtir.

```csharp
public int RefreshInternal { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyRefreshInternalDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örneği anlamlı kılmak için örnek veri ekle
            worksheet.Cells["A1"].Value = "Connection Demo";
            
            try
            {
                // Veri bağlantısı oluştur (temel ExternalConnection sınıfını kullanarak)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // RefreshInternal özelliğini ayarla ve göster
                connection.RefreshInternal = 30; // Refresh every 30 minutes
                Console.WriteLine("RefreshInternal value: " + connection.RefreshInternal);
                
                // Yenileme aralığını değiştir
                connection.RefreshInternal = 60;
                Console.WriteLine("Updated RefreshInternal value: " + connection.RefreshInternal);
                
                // Bağlantı ayarlarıyla çalışma kitabını kaydet
                workbook.Save("RefreshInternalDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


